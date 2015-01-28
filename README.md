# phpmemcachedadmin-debian
Debian Packaging information for phpmemcachedadmin

https://code.google.com/p/phpmemcacheadmin/

## TODO
* test lighttp-configuration
* read the debian-manuals to get this to the repositories

## HOWTO
```bash
cd
mkdir phpmemcachedadmin
cd phpmemcachedadmin
git clone https://github.com/krumedia/phpmemcachedadmin-debian.git phpmemcachedadmin_1.2.2
wget https://phpmemcacheadmin.googlecode.com/files/phpMemcachedAdmin-1.2.2-r262.tar.gz
tar xzf phpMemcachedAdmin-1.2.2-r262.tar.gz -C phpmemcachedadmin_1.2.2
mv phpMemcachedAdmin-1.2.2-r262.tar.gz phpmemcachedadmin_1.2.2.orig.tar.gz
cd phpmemcachedadmin_1.2.2
rm README.md
debuild
```
