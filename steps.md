# Installing *Git* on *Linux*

## Debian-based linux systems

```shell
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install git
```

## Red Hat-based linux systems


```shell
sudo yum upgrade
sudo yum install git
```

*Check git command now*

```shell
git help
```

# Installing Go on Linux machine

> Go is an open source programming language that makes it easy to build simple, reliable, and efficient software. 
> Visit https://golang.org

Note: We're going to install Go version `1.10.3`

### Download Go source

```shell
wget https://dl.google.com/go/go1.10.3.linux-amd64.tar.gz
```

### Unpack Go source

```shell
sudo tar -C /usr/local -xzf go1.10.3.linux-amd64.tar.gz
```

### Add go binary path to the system path

Open `$HOME/.profile` file
```shell
gedit $HOME/.profile   
```
Add following line to the bottom of $HOME/.profile file

```shell
export PATH=$PATH:/usr/local/go/bin
```

Try it out:
```shell

go help
```

Find GOPATH
```shell
go env | grep GOPATH

```
Create project hierarchy like:

```shell
~/go$ tree 
.
└── src
    └── github.com
        └── satyamz

```