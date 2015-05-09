Go
=========

This role installs (downloads) the Go programming language and adds it to the PATH system wide.

Install location:

	/usr/local/go


Requirements
------------

The remote nodes should have internet access and tar utility present.


Role Variables
--------------
go: (OPTIONAL - defined in defaults/main.yml)

defaults/main.yml:
```
go:
 download_url: "https://storage.googleapis.com/golang"
 src_file_name: "go1.4.2.linux-amd64.tar.gz"
 src_file_sha256: 141b8345932641483c2437bdbd65488a269282ac85f91170805c273f03dd223b
```

Dependencies
------------

* Internet access on remote
* tar


Example Playbook
----------------


- hosts: servers
  roles:
   - Go


Author Information
------------------

Tal Lannder

Tal@Pjili.com
