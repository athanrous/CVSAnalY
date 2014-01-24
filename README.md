# CVSAnaly

## Description

The CVSAnalY tool extracts information out of source code repository logs and stores it into a database.


## License

Licensed under GNU General Public License (GPL), version 2 or later.


## Download

* Home page: https://github.com/MetricsGrimoire/CVSAnalY
* Releases: https://github.com/MetricsGrimoire/CVSAnalY/downloads
* Latest version: `git://github.com/MetricsGrimoire/CVSAnalY.git`


## Requirements

CVSAnalY has the following dependencies:

* Python >= 2.5
* RepositoryHandler: `git clone git://github.com/MetricsGrimoire/RepositoryHandler.git`
* CVS (optional, for CVS support)
* Subversion (optional, for SVN support)
* git (optional, for Git support)
* Python MySQLDB (optional, but recommended)



## Requirements (Mac OS X)

CVSAnalY has the following dependencies (tested in Mac OS X 10.9.1 x86_64):

* XCode. Folow the instructions [given] [a] 
* MacPorts. Follow the instructions [given] [b] 
* Homebrew. Follow the instructions [given] [c]

After the installation open your terminal and type : 

For CVS support :

	$ brew install cvs

For Subversion support :

	$ brew install svn
	
For Git support :

	$ brew install git
	
	

* MySQL (mysql-server). Follow the official [MySQL Documentation] [d]
* python-mysqldb. Follow the instruction given in the [Stackoverflow thread] [e] 


[a]: https://developer.apple.com/xcode/
[b]: http://guide.macports.org/#installing
[c]: http://brew.sh/
[d]: http://dev.mysql.com/doc/mysql-macosx-excerpt/5.5/en/
[e]: http://stackoverflow.com/questions/1448429/how-to-install-mysqldb-python-data-access-library-to-mysql-on-mac-os-x



## Scripts

Some useful scripts for performing reseach studies (activity,
generations, etc) can be found in the next link:

        http://git.libresoft.es/libcvsanaly2

You can get the code from the git repository:

        git clone git://git.libresoft.es/git/libcvsanaly2
        git clone http://git.libresoft.es/libcvsanaly2


## Installation

You can install cvsanaly2 just by running setup.py script:

    # python setup.py install

This will install it in the python default directories in your system.

If you don't install CVSAnalY with root privileges, or don't want
to install it in the default directories, you can also use the source
code directory, as cloned from the main git repo. It is enough to
configure your PATH and PYTHONPATH so that cvsanaly2, and the Python
modules it needs, are found.

Add to your $PATH the directory which contains cvsanaly 
(cvsanalydir is the directory where CVSAnalY is installed):

    $ export PATH=$PATH:cvsanalydir

In PYHTONPATH, you need to include both the dirs for CVSAnalY and
RepositoryHandler (except if it is installed in the default Python dirs
in your system). If repohandlerdir is the path where RepositoryHandler
is installed:

    $ export PYTHONPATH=$PYTHONPATH:cvsanalydir:repohandlerdir

You are ready to use cvsanaly2!


## Running cvsanaly2

For the impatients: just checkout (from svn or cvs) to obtain a local
version of your repository, and then run cvsanaly2:

    $ cd project/
    ~/project$ cvsanaly2 

More options, and a more detailed info about the options, can be
learnt by running "cvsanaly2 --help"


## Useful settings

* Raise your `max_allowed_packet`-setting of your database (MySQL). 1 or 16 MB might be to low (depends on your repository)


## Analysis

[To be written]


## Improving CVSAnalY

Source code, wiki and ITS available on Github: https://github.com/MetricsGrimoire/CVSAnalY

If you want to receive updates about new versions, and keep in touch with the development team, consider subscribing to the mailing list. 
It is a very low traffic list (< 1 msg a day): https://lists.libresoft.es/listinfo/metrics-grimoire


## Credits

CVSAnalY was initially developed by the GSyC/LibreSoft group at the Universidad Rey Juan Carlos, Madrid (Spain). 
It is part of a wider research on libre software engineering, aimed to gain knowledge on how libre software is developed and maintained.


## Main authors

* Carlos Garcia Campos (carlosgc at gsyc.es)


## Contributors

* Gregorio Robles (grex at gsyc.escet.urjc.es)
* Alvaro Navarro (anavarro at gsyc.escet.urjc.es)
* Jesus M. Gonzalez-Barahona (jgb at gsyc.escet.urjc.es)
* Israel Herraiz (herraiz at gsyc.escet.urjc.es)
* Juan Jose Amor (jjamor at gsyc.escet.urjc.es)
* Martin Michlmayr (tbm at debian.org)
* Alvaro del Castillo (acs at barrapunto.com)
* Santiago Dueñas (sduenas at libresoft.es)
* and a lot of other [awesome contributer via github](https://github.com/MetricsGrimoire/CVSAnalY/graphs/contributors)
