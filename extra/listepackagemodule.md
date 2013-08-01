Date: 2013-05-29
Title: Lister package et modules python
Category: Geek
Tags: python,packages,package,list,lister,ubuntu

Comment lister les packages ubuntu installes :


	#!/usr/bin/env
	dpkg --get-selections > packages.txt


Comment lister les modules pythons installes :


	#!/usr/bin/env
	python -c "help('modules')" > modules.txt


