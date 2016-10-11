Set system time to local:

	$ sudo dpkg-reconfigure tzdata

Add pubkeys for any machines requiring access to ~/.ssh.authorized_keys:

	$ scp ~/.ssh/authorized_keys root@host:~/.ssh/

Remove password authentication for SSH:

	$ vim /etc/ssh/sshd_config

Set:

	PasswordAuthentication no

Configure git:

	$ git config --global user.name "John Doe"
	$ git config --global user.email johndoe@example.com
