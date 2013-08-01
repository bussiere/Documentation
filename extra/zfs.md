Date: 2013-05-29
Title: Zfs
Category: Geek
Tags: zfs,unix,ubuntu,linux

Quelques commandes utiles pour zfs :


Faire un snapshot recursif et le zipper :
	
	#!/usr/bin/env
	zfs snapshot -r rpool/ROOT/ubuntu-1@july
	zfs send rpool/ROOT/ubuntu-1@july | gzip > july.gz 

Revenir en arriere :
	
	#!/usr/bin/env
	zfs rollback tank/home/ahrens@tuesday

Envoyer et recevoir une image :

	#!/usr/bin/env
	zfs send tank/gozer@0830 > /bkups/gozer.083006
	zfs receive tank/gozer2@today < /bkups/gozer.083006
	zfs rename tank/gozer tank/gozer.old
	zfs rename tank/gozer2 tank/gozer