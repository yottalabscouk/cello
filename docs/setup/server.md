## 1. System Requirement

* Hardware: 4c8g100g
* Linux Kernel >= 3.0.0
* Docker engine: 17.15.5+
* docker-compose: 1.24.1+

## 2. Setup Steps

### 2.1 Clone source code

Ubuntu 18.04+:
```
sudo apt install git
```
```
git clone https://github.com/hyperledger/cello.git
```
### 2.2 Prepare environment

Ubuntu 18.04+:
```
sudo apt install make
```

```
# it takes few minutes
make docker
```

```
# quick check if hyperledger/cello-nginx and hyperledger/cello-api-engine have been created
docker images
```
```
# requires Python 2.7
sudo apt install python
```
```
make menuconfig
```

### 2.3 Start service

```
make start
```
```
# check running containers
docker ps -a

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
