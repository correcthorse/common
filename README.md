correcthorse.common
=========

This role contains some basic common tasks/handlers. This includes some tasks for installing the EPEL and IUS repositories as well as some handlers for systemd and firewalld. You can optionally install the correcthorse packagecloud repo. This may be enabled by other roles that depend on it.

Role Variables
--------------
| Variable                              | Default                       | Notes                                         |
| :---                                  | :---                          | :---                                          |
| common_install_correcthorse           | false                         | install correcthorse packagecloud repo	|
| common_epel_exclude			| ''				| exclude epel pkgs - useful if using upstream repos |

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: correcthorse.common }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)
