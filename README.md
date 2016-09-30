R-Project
=========

Install the latest version of R. If you need a graphical editor, this role can install: R Commander and R Studio. 

R Project:https://www.r-project.org/\n
R Studio: https://www.rstudio.com/
R Commander: http://www.rcommander.com/

Role Variables
--------------
- ```install_rcommander```: Whether or not install R Commander. Default: ``` false```.
- ```install_rstudio```: Whether or not install R Studio. Default: ``` false```.

Example Playbook
----------------

Install R and R Commander:
```yml
- hosts: all
  roles:
    - { role: 'serlophug.Rproject', install_rcommander: true}
```

Install R and R Studio:
```yml
- hosts: all
  roles:
	 - { role: 'serlophug.Rproject', install_rstudio: true}
```


License
-------

GNU General Public License v2 [1]

[1] https://www.r-project.org/COPYING
