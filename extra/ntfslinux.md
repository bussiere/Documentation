Date: 2013-08-05
Title: Ntfs et Linux
Category: Geek
Tags: ntfs,linux,formater,monter,mount,format

Comment formatter un disque dur en ntfs :

	#!/usr/bin/env
	# Comment formatter en ntfs
	$  mkntfs /dev/sde1

Comment monter un disque dur ntfs :

    #!/usr/bin/env
    # Comment monter un disque dur ntfs
    $ mount -t ntfs -o nls=utf8,umask=0222 /dev/hdb1 /media/c

