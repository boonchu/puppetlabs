my_firewall

Description
===========

my_firewall - Testing Puppetlabs firewall 

Use Case
========
 * Turn on firewall
 * enable port 22
 * enable port 80
 * add public network for test case port 80, assigned 192.168.1.103/24 address for public IP

```
config.vm.network :public_network, :bridge => $network_interface_to_use, :ip => '192.168.1.103'
```

How to run
==========

```
$ bundle install && bundle update && bundle exec rake spec_prep && bundle exec rake spec
$ vagrant up --provision
```

Pending Issues
==============
 * https://tickets.puppetlabs.com/si/jira.issueviews:issue-html/MODULES-1303/MODULES-1303.html
 * https://tickets.puppetlabs.com/browse/MODULES-1840

```
[Tue Aug 25 16:55:03.186560 2015] [:error] [pid 8172] [remote 192.168.1.151:220] mod_wsgi (pid=8172): Target WSGI script '/var/www/cgi-bin/hello.wsgi' does not contain WSGI application 'application'.
```

  * http://stackoverflow.com/questions/14410455/setting-up-python-with-wsgi-on-apache-for-a-directory


Platform
--------
 * work from CentOS 7

License Advisory
================
 * https://github.com/btford/participating-in-open-source