# VMware-Snort3
VMware Debian 8.1 image with snort3 and snort2 preconfigured.


###  Download 
Download virtual machine image @ [snort][mega]


### Login
To login digit: 
* “user”, as username, 
* “password”, as password.

### Root
To execute root operations, digit “su” command and then write “toor” as password.


### Running snort:

snort3 version 1.67: 
```
$ snort
```
snort3 version 1.72:  
 ```
$ snort3.172
```
snort2 version 2.976: 
 ```
$ snort2
```

##### N.B. 
Before lunching snort3 in IDS mode, don't forget to set LUA variables:
 ```
$ export LUA_PATH=$SNORT3_PATH/include/snort/lua/\?.lua\;\;
$ export SNORT_LUA_PATH=$SNORT3_PATH/etc/snort
```

[mega]: <https://mega.nz/>



