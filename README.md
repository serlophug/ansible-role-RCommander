[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Build Status](https://travis-ci.org/serlophug/ansible-role-Rproject.svg?branch=master)](https://travis-ci.org/serlophug/ansible-role-Rproject)
R-Project
=========

Install the latest version of R. If you need a graphical editor, this role can install: R Commander and R Studio. 

R Project: https://www.r-project.org/<br />
R Studio: https://www.rstudio.com/<br />
R Commander: http://www.rcommander.com/<br />

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
