puppet-install-shell
====================

A fork from https://github.com/petems/puppet-install-shell

A shell script to install puppet on multiple distros, assuming no dependencies.

The code is a mashup of [puppet-bootstrap](https://github.com/hashicorp/puppet-bootstrap) and [chef's install.sh script](https://www.getchef.com/chef/install.sh).

Usage
```
$ ./puppet.sh [-p] [-v version] [-f filename | -d download_dir]
```

Defaults to latest available as a version if none is given.

Currently working on: Debian, CentOS.

A quick way to install after carefully looking at the source:

Puppet < 3.8.X

```
$ wget -O - https://raw.githubusercontent.com/opinkerfi/puppet-install-shell/master/install_puppet.sh | sudo sh
```

Puppet > 4.X
```
$ wget -O - https://raw.githubusercontent.com/opinkerfi/puppet-install-shell/master/install_puppet_agent.sh | sudo sh
```
