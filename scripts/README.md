##### Puppet scripts

* git clone 
* review Gemfile 
   - modify code to have --parser future if run puppet version 3.7.x
* bundle install

##### Samples

```
* puppet-lint hello.pp
* puppet parser validate hello.pp
* run ./hello.pp
```

```
* puppet-lint --no-autoloader_layout-check array.pp
* puppet parser [--parser future] validate array.pp
* run ./array.pp
```

```
* puppet-lint --no-autoloader_layout-check reduce.pp
* puppet parser [--parser future] validate reduce.pp
* run ./reduce.pp
```

```
* puppet module install puppetlabs-ntp
* puppet module list
* puppet config print modulepath
```
