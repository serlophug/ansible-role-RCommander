Role Name
=========

Install the latest version of R. If you need the graphical editor R Commander, this role can install it. 


Role Variables
--------------
- ```install_rcmdr```: Whether or not install R Commander. Default: ``` true```.

Example Playbook
----------------

Install R and R Commander:
```yml
- hosts: all
  roles:
    - { role: 'serlophug.RCommander'}
```

Install R:
```yml
- hosts: all
  roles:
	 - { role: 'serlophug.RCommander', install_rcmdr: false}
```


License
-------

GNU General Public License v2 [1]

[1] https://www.r-project.org/COPYING