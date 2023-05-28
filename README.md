# install
install.camel-k.com - install on fedora 


+ [camelexamples](https://github.com/camelexamples)


### Prepare the Environment:

+ proxmox - [Download Proxmox software, documentation, agreements](https://www.proxmox.com/en/downloads)
+ fedora server iso - [Fedora Server - The Fedora Project](https://fedoraproject.org/server/download/)




## Run

+ [Download - JBang](https://www.jbang.dev/download/)
+ [Getting Started :: Apache Camel](https://camel.apache.org/manual/getting-started.html)




## [Camel + JBang: bringing the world of Java scripting to Camel - Apache Camel](https://camel.apache.org/blog/2021/07/camel-jbang/)

install jbang

```bash
curl -Ls https://sh.jbang.dev | bash -s - app setup
```


```bash
sudo dnf copr enable @jbangdev/jbang 
```

```bash
sudo dnf install -y jbang
```


```bash
sudo dnf update -y
```

For Linux, macOS, and Windows (using WSL or bash compatible shell like Cygwin or MinGW)

```bash
curl -Ls https://sh.jbang.dev | bash -s - trust add https://github.com/apache/
curl -Ls https://sh.jbang.dev | bash -s - app install --fresh --force camel@apache/camel
```


## Create your first Camel integration

```bash
camel init hello.java
```

## Run the Camel integration

``` bash
camel run hello.java
```

Bang the Camel integration is now running. You can use ctrl + c to stop the integration.

Camel makes it easy to change your code on the fly. You can run in live coding mode, as shown:

```bash
camel run hello.java --dev
```

While in live coding mode, whenever you save changes to hello.java, Camel will automatically load the updated version.


create project
```
mkdir example
cd example
jbang init hello.java
```

create
```
jbang hello.java
```

update
```bash
jbang edit --open=[editor] hello.java
```

verify JBang
```
jbang version
```

to use Camel JBang then install the following:
```
jbang app install camel@apache/camel
```



## Enable shell completion

Camel JBang provides shell completion for bash and zsh out of the box. To enable shell completion for Camel JBang, run:

```
source <(camel completion)
```

To make it permanent, run:
```
echo 'source <(camel completion)' >> ~/.bashrc
```



## instal k3c and Camel

+ [K3s](https://k3s.io/)

```bash
curl -sfL https://get.k3s.io | sh - 
```

Check for Ready node, takes ~30 seconds 
```bash
sudo k3s kubectl get node 
```




---

+ [edit](https://github.com/camel-k-examples/install/edit/main/README.md)
