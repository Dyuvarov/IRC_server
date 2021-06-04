# IRC SERVER "IRISHA" 👧🏼

## Introduction
IRC (Internet Relay Chat) - is an application layer protocol that facilitates communication in the
form of text. Was very popular in 90-s. People used IRC to communicate long before facebook, telegram, whatsApp e.t.c.
Read about it on [Wiki](https://en.wikipedia.org/wiki/Internet_Relay_Chat).

## This project is about
* Sockets
* Client-server interaction
* Server-server interaction

## Main part
Irisha work according to the IRC RFCs: [1459](https://datatracker.ietf.org/doc/html/rfc1459),
[2810](https://datatracker.ietf.org/doc/html/rfc2810),
[2811](https://datatracker.ietf.org/doc/html/rfc2811),
[2812](https://datatracker.ietf.org/doc/html/rfc2812),
[2813](https://datatracker.ietf.org/doc/html/rfc2813).
It means that users can connect to the network using any client works according to the RFC
([HexChat](https://en.wikipedia.org/wiki/HexChat) for example).
Irisha can connect to other IRC servers and create the IRC network (tested with ngIRCd).

## How to launch

#### Configuration
The `irisha.conf` file is used for server-settings. You can find configuration instructions [here](CONFIGURATION.md)

#### Execution
1) Run "make" command to compile project in the root.
2) Execute "ircserv" (./ircserv in terminal) with arguments
    * ./ircserv "port" "password" - if you want to start server and create new network
    * ./ircserv "hostname:network_port:network_password port password" -
      if you want to connect to other server

Other possibilities:
* make clean - delete all .o file
* make fclean - delete all .o file and execution file
* make re - recompile project

## ❗
Tested on MacOS.