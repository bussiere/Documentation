Date: 2013-07-24
Title: Decouper un fichier avec 7z
Category: Geek
Tags: 7z,compression,decoupe,cryptage,cryptographie


Pour decouper un fichier en archive de 2048M (utile quand le systeme de fichier ne prends pas plus de 4 gigas pour les fichiers.) :


	#!/usr/bin/env
	# Comment decouper :
	$ 7z a -v2048m -mx0 Secretaire.7z Secretaire.mkv
	# Comment decouper ET crypter :
	$ 7z a -mhe=on -pMotdePasse -v90m -mx0 Emmanuel.7z Emmanuel/


