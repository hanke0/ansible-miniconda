ko-han.ansible_miniconda
=========

Installs [Miniconda](https://conda.io/miniconda.html) use ansible


Role Variables
--------------
```yml
# miniconda download url
miniconda_installer_url: https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh

# miniconda installer file full path
miniconda_installer_file: /tmp/miniconda.sh

# miniconda install to this path
miniconda_path: /usr/local/miniconda

miniconda_bin: '{{ miniconda_install_path }}/bin/conda'

# add miniconda to path
miniconda_activate_in_bashrc: yes

# become root if necessary
miniconda_use_sudo: yes

```

Example Playbook
----------------

```yml
- hosts: servers
  roles:
    ko_han.ansible_miniconda
```

How to install
----------------

```bash
ansible-galaxy install ko_han.ansible_miniconda
```

License
-------

MIT
