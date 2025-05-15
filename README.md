# My Ansible Collection

**Requirements**
- Something needs to parse over the hosts inventory files to ensure all hosts contain all the same entries with different values.
- When deploying the changes to Ansible, something should automatically create the respective objects inside Ansible so it's not manual, and will be consistent.
  - The hosts files should be registered automatically as inventories.
  - The playbooks could all be registered as job templates with the inventory automatically checking for all inventories present. Eg: Activate (Prod1), Up (Prod1), etc.

**Notable Changes:**
- The `ansible.cfg` file does contain the `roles_path` setting to ensure the roles stays at the root of the collection, and is not relative to the playbooks.
