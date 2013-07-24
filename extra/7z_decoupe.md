Date: 2013-07-24
Title: Decouper un fichier avec 7z
Category: Geek
Tags: 7z,compression,decoupe


Pour decouper un fichier en archive de 2048M (utile quand le systeme de fichier ne prends pas plus de 4 gigas pour les fichiers.) :


	#!/usr/bin/env
	7z a -v2048m -mx0 Secretaire.7z Secretaire.mkv


