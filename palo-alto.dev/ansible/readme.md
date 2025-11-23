## Prep Environment ##

# Install the PAN-OS Ansible collection #

```
ansible-galaxy collection install paloaltonetworks.panos
```

# Install pandevice dependencies (if not already installed) #

```
pip install pan-os-python
```

# Set environment variables (optional but recommended for credentials) #

```
export PAN_HOST=192.168.1.1
export PAN_USERNAME=admin
export PAN_PASSWORD=yourpassword
```

# Now run the playbook

```
ansible-playbook -i inventory.yml get_fw_info.yml
```