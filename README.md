# Ansible Role: pgporada.repo-sysdig
This role will install and configure the [Sysdig](https://github.com/draios) repository. http://www.sysdig.org/

- - - -
# Example Playbook

If running this locally

    ---
    - hosts: localhost
      connection: local
      become: true
      become_method: sudo
      roles:
        - ansible-role-repo-draios

Run the playbook as follows

    ansible-playbook -i localhost -c local example_playbook.yml

- - - -
# Music

[Bedouin Soundclash - Walls Fall Down](https://www.youtube.com/watch?v=E0M0L6oueUY)

- - - -
# Author Information and License
GPLv3

(C) 2016 - [Phil Porada](https://philporada.com)
