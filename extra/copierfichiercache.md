Date: 2013-08-05
Title: Copier les fichiers caches et repertoires
Category: Geek
Tags: administration,hidden,file,copie,copy,regex

Comment copier les fichiers caches et repertoires :

	#!/usr/bin/env
	# Comment copier les fichiers et repertoires caches
	$ cp -r .[^.]* workspace/Configuration/
