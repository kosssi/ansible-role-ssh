# ansible-role-ssh

Ansible role to install and configure ssh.

## Role Defaults Variables

    ssh_packages:
      - openssh-client
      - openssh-server

    ssh_authorized_keys:
      - name: www-data
        home: /var/www
        local:
          -  "~/.ssh/id_rsa.pub"

## Example Playbook

    roles:
      - { role: kosssi.ssh, tags: php }

## License

Licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
