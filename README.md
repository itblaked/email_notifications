Email Notifications
=========

This role sends email notifications.

Role Variables
--------------

```yaml
# These variables map directly to the parameters of the mail module, details on their purpose can be read on the module page:

# https://docs.ansible.com/ansible/latest/collections/community/general/mail_module.html

mail_host:
mail_password:
mail_username:
mail_attach:
mail_body:
mail_cc:
mail_port:
mail_secure:
mail_sender:
mail_subject:
mail_subtype:
mail_to:

```

Dependencies
------------

This role depends on the `community.general` collection.

Example Playbook
----------------

```yaml
- name: Send email notifications
  hosts: localhost
  connection: local
  gather_facts: no
  tasks:
    - name: Apply email_notifications role
      include_role:
        name: email_notifications

```

License
-------

BSD

Author Information
------------------

Blake Douglas, blake@redhat.com
