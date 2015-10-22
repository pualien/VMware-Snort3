# VMware-Snort3
VMware Debian 8.1 image with snort3 and snort2 preconfigured.


###  Download 
Download virtual machine image @ [Debian 8.1+snort3+snort2.zip][mega]


### Login
To login digit: 
* “user”, as username, 
* “password”, as password.

### Root
To execute root operations, digit ```$ su``` command and then write “toor” as password.


### Running snort as root:

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

## Notes

####snort3 environment
Before lunching snort3, don't forget to set up the environment:
 ```
$ export LUA_PATH=$SNORT3_PATH/include/snort/lua/\?.lua\;\;
$ export SNORT_LUA_PATH=$SNORT3_PATH/etc/snort
```

#### Installing next versions of snort3
```
$ git clone git://github.com/snortadmin/snort3.git
$ cd snort3/
$ mkdir -p /path/to/snorty
$ export my_path=/path/to/snorty
``` 
/path/to/snorty could be for example: /opt/snort3_new_version
```
$ ./configure --prefix=$my_path && make -j 8 install
```


[mega]: <https://mega.nz/#!UkwUCKDb!6_6JpTcqrzd0BlRAvPwbBDK6hcrFdlTumaGXFr1aGnA>



