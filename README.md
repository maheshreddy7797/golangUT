# Install GoLang on VM

A [Vagrantfile](https://github.com/maheshreddy7797/golangUT/blob/master/Vagrantfile) is placed that can install Golang software on ubuntu VM.

## Prerequisites

```
-Laptop/Desktop with Linux distribution, preferably Ubuntu 16.04 LTS
-Vagrant version  ('>= 1.9.1')
-Virtualbox       ('>= 5.1')
-Git
```
    
## Install GO using vagrant file


```
~$ cd /path/to/your/working/directory
~$ git clone https://github.com/maheshreddy7797/golangUT
~$ cd golangUT
~$ vagrant up
~$ vagrant ssh
```

After doing successful vagrant up GoLang has been installed in the VM.

## Check Go Installation on VM and set Go variables

```
vagrant@GoLang:~$ go version
go version go1.6.2 linux/amd64
vagrant@GoLang:~$ export GOPATH= /home/vagrant/go
vagrant@GoLang:~$ export GOROOT= /usr/local/go
```

## Running Go files present in this repository

```
    vagrant@GoLang:~$ git clone https://github.com/maheshreddy7797/golangUT
    vagrant@GoLang:~$ cd golangUT
    vagrant@GoLang:~$ go test -coverprofile = ./
    ok  	_/home/vagrant/golangUT	0.005s	coverage: 100.0% of statements
```
