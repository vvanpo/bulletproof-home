
Potential feature list
----------------------

- File tracker interface (GUI, TUI, and CLI?), ability to mark and unmark files for syncing (much like VCS, but without the history)
	- Nautilus plugin
		- Automatic folder organization?
		- Camera imports
	- Music tags, folder heirarchy
	- Tracked file metadata VCS?  (using git object-store or sqlite)
- Control and consistency of UNIX permissions
- Transparent encryption/decryption
	- Encfs/Fuse?
	- Password-protected folders, integrated with PAM, integrated with password managers like pass?
- Rsync-able files, block encryption on said files compatible with rsync protocol
- P2P, a la btsync ?
- Incremented, compressed backups on server or external drive; automatic when plugged in or connected
- Automatic handling of command aliases and shell idiosynrasies on incompatible systems
- Track private-key/password -> service mappings, panic button to archive all private-keys/passwords, create new ones, and update services

Existing technologies
---------------------

- [csync](https://www.csync.org/)
	- Client-only sync using sftp/smb
	- "Floating home directory"
	- PAM integration
	- Development has stalled, may have moved to ownCloud?
- [ownCloud](http://owncloud.org)
	- Client/server architecture
- [btsync](http://www.bittorrent.com/sync)
	- Proprietary
	- Torrent-based file transfer, unique key is stored in the DHT meaning all synced clients are publicly linked
- [duplicity](http://duplicity.nongnu.org/)
- [Dropbox](https://www.dropbox.com)
	- Proprietary
	- No control over hosting or server-side encryption
- [git-annex](https://git-annex.branchable.com/walkthrough/)
- [Seahorse](https://wiki.gnome.org/Apps/Seahorse)

Research and Links
------------------

- [Keeping private GPG keys safe](https://alexcabal.com/creating-the-perfect-gpg-keypair/)
- [Linux-PAM application dev's guide](http://www.linux-pam.org/Linux-PAM-html/Linux-PAM_ADG.html)
- [PAM bindings for Go](https://code.google.com/p/gopam/source/browse/)
- [libev](http://software.schmorp.de/pkg/libev.html)
- [Git object store](http://git-scm.com/book/en/Git-Internals-Git-Objects)
- [User-mode NFS for Linux](https://github.com/nfs-ganesha/nfs-ganesha)
