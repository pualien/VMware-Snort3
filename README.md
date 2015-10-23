# VMware-Snort3
VMware Debian 8.1 image with snort3 and snort2 preconfigured:

* Memory: 724 MBytes
* Processor: 1
* Hard Disk: 50 GBytes (6.1 GBytes occupied, 41.9 GBytes free)
* Network Adapter: NAT

Feel free to customize these settings.


###  Download 
Download virtual machine image @ [Debian 8.1+snort3+snort2.zip][mega] size: 2.32 GBytes, uncompressed 6.56 GBytes.


### Login
To login digit: 
* “user”, as username, 
* “password”, as password.

### Root
To execute root operations, digit ```$ su``` command and then write “toor” as password.


### Running snort as root

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

### Notes

#####Snort3 environment
Before lunching snort3, don't forget to set up the environment:
 ```
$ export LUA_PATH=$SNORT3_PATH/include/snort/lua/\?.lua\;\;
$ export SNORT_LUA_PATH=$SNORT3_PATH/etc/snort
```

##### Installing next versions of snort3
Download snort3 from official repository:
```
$ git clone git://github.com/snortadmin/snort3.git
$ cd snort3/
```
Create and define installation folder:
```
$ mkdir -p /path/to/snorty
$ export my_path=/path/to/snorty
``` 
/path/to/snorty could be for example: /opt/snort3_new_version

Configure and install into my_path:
```
$ autoreconf -isvf
$ ./configure --prefix=$my_path && make -j 8 install
```
Create link to lunch snorty in terminal:
```
$ su ln -s /path/to/snorty/bin/snort /usr/sbin/snorty
```

##### Installing next versions of snort2
Easy download and install stable snort2 releases through apt-get:
```
$ su apt-get install snort
```

[mega]: <https://mega.nz/#!UkwUCKDb!6_6JpTcqrzd0BlRAvPwbBDK6hcrFdlTumaGXFr1aGnA>



