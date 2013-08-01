Date: 2013-07-01
Title: Decouper un fichier avec gz
Category: Geek
Tags: gz,file,decouper,compression,cut

Comment decouper un fichier mais peut poser probleme sous windows pour cause d'absence de la commande cat

	#!/usr/bin/env
	# create archives
	$ gzip -c my_large_file | split -b 1024MiB - myfile_split.gz_
	# uncompress
	$ cat myfile_split.gz_* | gunzip -c > my_large_file