# How to Access VM Ports

Due to firewall restrictions, not all ports are open.
We need to use port forwarding to access ports that are closed by default.

## Setup VSCode SSH Config

1. Open VSCode.
2. Install the Remote - SSH extension if not already installed.
3. Open your SSH config file:

   ```sh
   vim ~/.ssh/config
   ```

4. Add the following lines to the file (replace the placeholders with your own values for the jumphost and target host):

   ```ssh-config
   # Configuration for the jumphost
   Host jumphost
     HostName jumphost.example.com
     User your_jumphost_username
     IdentityFile ~/.ssh/jumphost_private_key

   # Configuration for the target host using the jumphost
   Host targethost
     HostName targethost.example.com
     User your_targethost_username
     IdentityFile ~/.ssh/targethost_private_key
     ProxyJump jumphost
   ```

5. Save and close the file.
6. Open the Command Palette (⇧⌘P) and select **Remote-SSH: Connect to Host...**.
7. Enter `targethost` (as specified in your SSH config).

### Using VSCode for Port Forwarding

1. Connect to the VM using VSCode.
2. Open the Terminal for the VM.
3. Click the **Ports** tab next to the Terminal tab.
4. Enable port forwarding.
   VSCode will ask you to authenticate using your GitHub account.
   Log in and approve VSCode to use GitHub.
   (You only need to do this once, unless you revoke the permissions.)
5. Once everything is approved, you should be able to see the **Forwarded Address** in VSCode.
   If you click the link, it will ask you to log in to GitHub to authenticate that you have permission to access the page.
   (The link visibility is private by default.)
6. If you want to change the link visibility, go to the VSCode **Ports** tab, find the port you want to access publicly, and change the visibility from **Private** → **Public**.

For more details, see the [VSCode Port Forwarding Documentation](https://code.visualstudio.com/docs/editor/port-forwarding).

## Manual Port Forwarding

### Step 1: Connect to the VM with Port Forwarding

Use the following command to connect to your VM:

```sh
ssh ubuntu@floating_IP -D 20000 -i ssh_key
```

Port 20000 is a random port that is not used by any service on your local machine or virtual machine.

### Step 2: Configure Network Settings

1. Go to your network settings.
2. Enable manual proxy:
   - In the SOCKS Proxy settings, select **SOCKS v5**.
   - Set the host to `127.0.0.1`.
   - Set the port to `20000` (the port used in Step 1).

### Step 3: Access the VM

Open your browser and enter the private IP of the VM with the port number to access the service:

```text
http://192.168.1.25:8080
```

For example, if your VM has private IP `192.168.1.25` and you want to access port `8080`.

**Important Note:**
Once you terminate the SSH session, make sure to remove the proxy settings; otherwise, you will not be able to access the internet from your machine.
While connected with port forwarding active, you should have internet access.
