#### -> anony (unknown) in amharic is "የማይታወቅ".
#### -> when black hat hackers do security test on some target, they will be unknown (anonymous)
#### -> this is because they are doing illegal things so they try to be anonymous ( የማይታውቅ ሰው ).
#### -> anonmity is simply using a fake profile, location, identity and so more.

---
# methods of anonymity

#### -> there are several way to be protect or to be anonymous on the internet.
#### -> there methods can change our identity, location or personality.


### 1, Proxy chains
### 2, Tor Network
### 3, VPN
### 4, Mac change\
### 5, Incognito
### 6, Secured OS
### 7, Temp Mail
### 8, Temp Phone Number

---
# 1, Proxy chains

## -> What is Proxy Server?


#### -> a proxy server is a system or router that provides a getway between user and the internet. there fore, it help to prevent cyber attackers from entering a private network.
#### -> proxy mean intermediary ( መካከለኛ ).
#### -> በ internet እና በኛ መሃል የሚገባ ነው.
#### -> ስለዚ ያ website or server የ proxy server ሩ ip ነው የሚኞረው.
#### -> ስለዚ ያ website or server እኛ ሳንሆን proxy server ሩ access እያደረገው መሆኑን ነው የሚያቀው.


## YOU            --->            Proxy          --->            Internet 
#### 192.168.1.110                        183.53.23.4                             183.53.23.4


#### -> ግን በ normal or proxy ሳንጠቀም access የምናደርግ ከሆነ ያ website or server የኛ ip ነው የሚኖረው.


## YOU            --->            Internet 
#### 192.168.1.110                        192.168.1.110


## ->Proxy chains


#### -> ብዙ proxy ስንጠቀም proxy chains ይባላል.
#### -> ግን proxy በበዛ ቁጥር የ internet speed ይቀንሳል.
#### -> proxy በበዛ ቁጥር በጣም anonymous እንሆናለን.


## -> Type of Proxy chains


### 1, Dynamic chain
### 2, Starict chain
### 3, Round Robin chain
### 4, Random chain


## 1, Dynamic chain

#### -> a proxy list given.
#### -> if any server not working it will be skipped.
#### -> if all server not working it will be broken and display error.

## 2, Strict chain

#### -> all proxy have to be up and working, but if 1 is not working it will display error.

## 3, Round Robin chain

#### -> it will skip 1 proxy is not working.
#### -> if all the proxy not working it will start again and check.

## 4, Random chain

#### -> it will choose some proxy randomly and create chain in rando order.
#### -> not working will be skipped.


## -> Demo

### -> 1, find some proxy server on google
####             - proxy servers free lists
### -> 2, open "/etc/proxychains4.conf"
####        - Turn on any kind proxy chain type you need.
####        - put your proxy server, like this

### protocol          ip                 port          user          password

#### http             192.12.23.4          8080
#### socks4         192.12.23.4          4545           josi              123abc
#### socks5          192.12.23.4          90

### -> 3, To use a proxy server
####       - add "proxychains4" in front of any command.
####        ex :- proxychains4 ping 192.12.23.4
####       - command is display time out a proxy server is not working.

---
# T.o.r (The Onion Routing) Network

#### -> in tor network, if one user is connect to tor network that user computer or phone is a node.
#### -> if one user connect to tor network and accessing some thing, a tor network is select randomly 3 nodes and given him and that user accessing some thing passes on this 3 nodes.

### first node  ===  " Entry node "
### second node  ===  "Relay node"
### last node  ===  " Exit node "

#### -> exit node is ከ tor network ወቶ ወደ internet የሚሂድበት ነው.
#### -> onion ( ሽንኩርት ) የተባለበት ምክንያት encryption የተደራረበ ስለሆነ እንዲሁም እያንዳንዱ layer ላይ encryption ስላለ ነው.
#### -> one user connect to tor network and accessing a server, that server is known as a tor exit node ip, not your ip.
#### -> tor network is better to anonymity.


## -> To Connect a Tor network


### 1, install tor.
####         - sudo apt install tor
### 2, clone [Torghost](https://github.com/SusmithKrishnan/torghost) on github.
### 3, install a requirements 
### 4, run Torghost
####          - sudo python3 torghost.py

---
# VPN

#### -> VPN means virtual private network
#### -> VPN is encrypt all your data.
#### -> so isp can not see your activity.
#### -> but some time a free vpns leak your data, so paid vpn is best for more anonymity.
#### -> ex :-    1, Nord vpn               2, Proton vpn

---
# Mac change

#### -> as we saw mac address can tell about our device.
#### -> so, if we change that we can change our device id.


## -> To change

#### -> we can use a linux tool called "macchanger".

### 1, Randomly

#### -> first turn off the interface
####         - sudo ifconfig wlan0 down
#### -> second change a mac
####          - sudo macchanger -r wlan0
#### -> last turn on the interface
####          - sudo ifconfig wlan0 up

## 2, Manually

#### -> turn off interface
#### -> change a mac
####           - sudo macchanger -m "mac" wlan0
#### -> turn on interface



#### -> To check
####            - sudo macchanger -s wlan0
#### -> To back a current mac
####       - sudo macchanger -p wlan0

---
# Online Privacy

### -> incognito or privacy tabs.
#### -> this type of tabs is not save your data, login or signin info or cookies, history all you doing on this tabs is gest for ones, if close this tab and open again your data is gone.
#### -> but your isp can see your activity.

---
# Secure OS

#### -> this are operating system, that have a security and privacy features.
#### -> windows and mac os will record some of your activity also they are not good on security and privacy.
#### -> there for the always best os is Linux is always recommanded when you think about privacy and security.

#### -> ex :-       1, tails os

---
# Temp Mail & Temp Phone number

#### -> you don't use personal email or phone number for some pentest( Hacking ).
#### -> but you can user Temp email and Temp phone number providers.


### For Email

#### -> search on google
####          - Temp mail
#### -> or you can use extension called
####           - Temp MAIL


### For Phone number

#### -> search on google
####            - Temp phone number 
#### -> or you can use extension called
####            - Temp Phone number

---
# Browser

#### -> Brave browser and dagedago search eagine, is the best and secure way to access a internet.

---
# Proton mail

#### -> Proton mail is a secure email service that emphasizes privacy and encryption.

---
# OPSEC

#### -> opsec stand for Operational Security.
#### -> ባጭሩ የናንተ መረጃ እንደ photo, phone number, location የመሳሰሉትን online ላይ or internet ላይ አለመልቀቅ እና የናንተ የትኛውም ትክክለኛ የሆነ ነገር internet ላይ መኖር የለበት. በሱ ፋንታ sock poppet, random identity or fake identity መጠቀም.
### -> Website:
####                  - [fakenamegenerator](https://www.fakenamegenerator.com)

---
# Tip

### -> Use Password Manager
### -> Full Anonymous Tool
####            - kali-whoami
