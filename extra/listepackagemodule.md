Date: 2013-08-01
Title: Lister package et modules python
Category: Geek
Tags: python,packages,package,list,lister,ubuntu

Comment lister les packages ubuntu installes :


	#!/usr/bin/env
	dpkg --get-selections > packages.txt


pour reinstaller sans le install dans les fichiers :

    aptitude install $(cat <textfile>)


Comment lister les modules pythons installes :


	#!/usr/bin/env
	python -c "help('modules')" > modules.txt


