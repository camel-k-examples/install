# install
install.camel-k.com - install on fedora 



### Prepare the Environment:

+ proxmox - [Download Proxmox software, documentation, agreements](https://www.proxmox.com/en/downloads)
+ fedora server iso - [Fedora Server - The Fedora Project](https://fedoraproject.org/server/download/)




## Run

+ [Download - JBang](https://www.jbang.dev/download/)
+ [Getting Started :: Apache Camel](https://camel.apache.org/manual/getting-started.html)



install jbang

```bash
curl -Ls https://sh.jbang.dev | bash -s - app setup
```


```bash
dnf copr enable @jbangdev/jbang 
dnf install jbang
```

For Linux, macOS, and Windows (using WSL or bash compatible shell like Cygwin or MinGW)

```bash
curl -Ls https://sh.jbang.dev | bash -s - trust add https://github.com/apache/
curl -Ls https://sh.jbang.dev | bash -s - app install --fresh --force camel@apache/camel
```

