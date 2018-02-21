A very simple firewalld role.

    - hosts: all
      user: root
      roles:
        - role: ansible-role-firewalld
          firewalld_allowed_ports:
            - '80/tcp'
            - '443/tcp'
