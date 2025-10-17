# Lab 2 – Automated Web Server Configuration

### Steps:
1. Run the playbook:
   ```bash
   ansible-playbook webserver.yml -i ../Lab1-Initial-Config/inventory
   ```

2. Verify:
   - Check Nginx status:
     ```bash
     systemctl status nginx
     ```
   - Open in browser: `http://<Managed-Node-IP>`
