Role Name
=========

Install the latest version of R. If you need more packages or the graphical editor R Commander, this role can install it. 


Role Variables
--------------
- ```packages```: Packages to install. Default: ``` []```. 
- ```install_rcmdr```: Whether or not install R Commander. Default: ``` true```.

Example Playbook
----------------

Install R:
```yml
- hosts: all
  roles:
	 - { role: 'serlophug.ansible-role-octave', install_rcmdr: false}
```

Install R and R Commander:
```yml
- hosts: all
  roles:
    - { role: 'serlophug.ansible-role-octave'}
```

Install R, R Commander and additional packages:
```yml
- hosts: all
  roles:
    - { role: 'serlophug.ansible-role-octave', packages: [abc.data, DidacticBoost] }
```

License
-------

GNU General Public License v2 [1]

[1] https://www.r-project.org/COPYING