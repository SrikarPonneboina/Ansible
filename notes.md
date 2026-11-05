# Ansible Configuration File Priority

Ansible looks for its configuration file (`ansible.cfg`) in a specific order of precedence. It applies the settings from the **first file it finds** and ignores the rest.

### 🔍 Search Order Priority

1. **`ANSIBLE_CONFIG` (Environment Variable)**
   * **Priority:** Highest
   * **Usage:** Points directly to a specific file path via your terminal environment.

2. **`./ansible.cfg` (Current Working Directory)**
   * **Priority:** Second 
   * **Usage:** ⭐ *Most commonly used.* Placed at the root of your project directory so configuration travels with your playbooks.

3. **`~/.ansible.cfg` (Home Directory)**
   * **Priority:** Third
   * **Usage:** Used for user-specific global configurations in your user's home folder.

4. **`/etc/ansible/ansible.cfg` (Default System Directory)**
   * **Priority:** Lowest
   * **Usage:** The global fallback configuration installed automatically by the package manager.
