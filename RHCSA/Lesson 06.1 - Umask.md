
Default file and directory permission depand on umask

Linux Umask Value:
==================

	[root@dektopX lesson06]# umask
	0022

	permission value:
	 dir: 755
	 file: 644

	Directory: (umsk calculation for dir)
	  777(Maximum)
	 0022(umask)
	--------
	 0755(default)

	File: (umask calculation for file)
	  666(maximum)
	 0022(umask)
	------
	 0644(default)

	 Regular user (student):
	 Directory
	 0777(Maximum)
	 0002 (umask)
	------
	 0775 (Default)

	File
	 0666(Maximum)
	 0002 (umask)
	------
	 0664 (Default)	


	 Temporary umask change:
	  [root@dektopX lesson06]# umask 0033
	Permanently umask change:
	 [root@dektopX lesson06]# vim /etc/profile
		:set nu
