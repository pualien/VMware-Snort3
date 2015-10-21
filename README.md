# VMware-Snort3
VMware Debian 8.1 image with snort3 and snort2 preconfigured.


###  Download 
Download virtual machine image @ [snort][mega]


### Login
To login digit: 
* “user”, as username, 
* “password”, as password.

### Root
To execute root operations, digit ```$ su``` command and then write “toor” as password.


### Running snort:

snort3 version 3.0.0-a2-167: 
```
$ snort3a
```
snort3 version 3.0.0-a2-172:  
 ```
$ snort3b
```
snort2 version 2.9.7.6 GRE (Build 285): 
 ```
$ snort2
```

##### Note: snort3 environment
Before lunching snort3 in IDS mode, don't forget to set up the environment:
 ```
$ export LUA_PATH=$SNORT3_PATH/include/snort/lua/\?.lua\;\;
$ export SNORT_LUA_PATH=$SNORT3_PATH/etc/snort
```

[mega]: <https://mega.nz/>



