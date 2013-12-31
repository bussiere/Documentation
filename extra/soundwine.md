Date: 2013-08-05
Title: Son et wine
Category: Geek
Tags: ntfs,linux,formater,monter,mount,format


Bad Sound in Wine 1.4 under Ubuntu 12.04 12.10 13.04 x64
Submitted by Jean-Paul on Sun, 05/06/2012 - 19:46

I did a lot of searching for a solution to this problem. Any programs that I would run with Wine had horrible sound. It was almost like an underrun or something like that. I unfortunately don't have output from the terminal, but thankfully I do have a solution, as posted on Wine's wiki. Just to be clear, the sound I was getting was kind of scratchy, like a "farting" noise. I would get the same scratchy sound when using winecfg's "test sound" button, and it didn't matter what options I chose. So, here's the fix!

1. Edit your /etc/pulse/daemon.conf

2. Scroll down to the line that reads "default-fragment-size-msec = 10"

3. Change the 10 to a 5 and save.

4. Restart pulseaudio or reboot. Maybe. I called "sudo /etc/init.d/pulseaudio restart" but got no output, so this might not be required.

5. Post a comment if this worked for you!

Comment formatter un disque dur en ntfs :

	#!/usr/bin/env
	# Comment formatter en ntfs
	$  mkntfs /dev/sde1

Comment monter un disque dur ntfs :

    #!/usr/bin/env
    # Comment monter un disque dur ntfs
    $ mount -t ntfs -o nls=utf8,umask=0222 /dev/hdb1 /media/c

