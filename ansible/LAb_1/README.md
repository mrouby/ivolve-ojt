# Lab 1 – Initial Ansible Configuration

### Steps:
1. Install Ansible on control node:
   ```bash
   sudo dnf install ansible-core -y
   ```

2. Generate SSH key:
   ```bash
   ssh-keygen
   ```

3. Copy key to managed node:
   ```bash
   ssh-copy-id root@192.168.137.132
   ```

4. Verify connection:
   ```bash
   ansible all -m ping
   ```

5. Run ad-hoc command to check disk space:
   ```bash
   ansible all -a "df -h"
   ```
