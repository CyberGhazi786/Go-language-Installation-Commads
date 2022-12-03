# Go-language-Installation-Commads
GO language Or Golang Installation Commands For ParrotSec OS / Kali / Ubuntu / Any Debian Linux


┌─[cyberghazi@cyberghazi-vmwarevirtualplatform]─[~/Downloads] Right Click and Open terminal
root@cyberghazi-vmwarevirtualplatform:/home/cyberghazi/Downloads# rm -rf /usr/local/go && tar -C /usr/local -xzf go1.19.3.linux-amd64.tar.gz

root@cyberghazi-vmwarevirtualplatform:/home/cyberghazi/Downloads# pluma ~/.profile
# ~/.profile add his code in the end of file:
export PATH=$PATH:/usr/local/go/bin

root@cyberghazi-vmwarevirtualplatform:/home/cyberghazi/Downloads# which ~/.bashrc # use which command to see bashrc file location If not works then use locate command

root@cyberghazi-vmwarevirtualplatform:/home/cyberghazi/Downloads# locate bashrc
/etc/bash.bashrc 
/etc/bashrc
/etc/skel/.bashrc
/home/cyberghazi/.bashrc # This one is our file location 
/usr/lib/parrot-skel/etc/skel/.bashrc
/usr/lib/python3/dist-packages/pexpect/bashrc.sh
/usr/share/base-files/dot.bashrc
/usr/share/doc/adduser/examples/adduser.local.conf.examples/bash.bashrc
/usr/share/doc/adduser/examples/adduser.local.conf.examples/skel/dot.bashrc
root@cyberghazi-vmwarevirtualplatform:/home/cyberghazi/Downloads# cd ..
root@cyberghazi-vmwarevirtualplatform:/home/cyberghazi# cd ..
root@cyberghazi-vmwarevirtualplatform:/home# cd ..

root@cyberghazi-vmwarevirtualplatform:/# pluma /home/cyberghazi/.bashrc
Add these lines in the last of file & save  / close
#Golang Paths In bashrc
export GOROOT=/usr/local/go
export GOPATH=$HOME/go
PATH=$PATH:$GOROOT/bin/:$GOPATH/bin

root@cyberghazi-vmwarevirtualplatform:/# go version
bash: go: command not found because we did not souce it or compile it :-)
root@cyberghazi-vmwarevirtualplatform:/# source ~/.profile
root@cyberghazi-vmwarevirtualplatform:/# source /home/cyberghazi/.bashrc
┌─[root@cyberghazi-vmwarevirtualplatform]─[/]
└──╼ #go version
go version go1.19.3 linux/amd64 # AlhamdulilAllah
┌─[root@cyberghazi-vmwarevirtualplatform]─[/]
└──╼ #go
Go is a tool for managing Go source code.

Usage:

	go <command> [arguments]
