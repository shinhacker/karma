
<p align="center">
    <img alt="karma" src="https://i.imgur.com/C3zISlU.gif"/>
    <p align="center">
        <a href="https://github.com/decoxviii/karma/releases/latest"><img alt="Release" src="https://img.shields.io/github/tag/decoxviii/karma.svg?style=flat-square"></a>
        <a href="https://github.com/evilsocket/ergo/blob/master/LICENSE.md"><img alt="Software License" src="https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square"></a>
    </p>
</p>

---


##### API: pwndb2am4tzkvold (dot) onion

Find leaked emails with your passwords.


#### Installation

Install dependencies (Debian/Ubuntu):
```
sudo apt install tor python3 python3-pip
```

Clone this repository, and:
```
git clone https://github.com/decoxviii/karma.git; cd karma
sudo -H pip3 install -r requirements.txt
python3 setup.py build
sudo python3 setup.py install
```


#### Usage

Start by printing the available actions by running `karma --help`. It's also necessary to restart the **Tor** service `sudo service tor restart`. Then you can perform the following tests:

1. Search emails with the password: `123456789`
```
karma search '123456789' --password -o test1
```

2. Search emails with the local-part: `johndoe`
```
karma search 'johndoe' --local-part -o test2
```

3. Search emails with the domain: `hotmail.com`
```
karma search 'hotmail.com' --domain -o test3
```

4. Search email password: `johndoe@unknown.com`
```
karma target 'johndoe@unknown.com' -o test4
```


#### Disclaimer

Usage this program for attacking targets without prior consent is illegal. It's the end user's responsibility to obey allapplicable local, state and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program.


#### Thanks

This program is inspired by the projects:
+ [pwndb_api](https://github.com/M3l0nPan/pwndb_api) by: M3l0nPan
+ [pwndb](https://github.com/davidtavarez/pwndb)     by: davidtavarez

---

**decoxviii**

**[MIT](https://github.com/decoxviii/karma/blob/master/LICENSE)**
