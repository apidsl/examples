
![logo.inframonit.com](https://logo.inframonit.com/1/cover.png)

# [bash.inframonit.com](https://bash.inframonit.com/) [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/apidsl/examples/edit/main/DOCS/MENU.md) 

+ [Example usae cases - examples.inframonit.com](http://examples.inframonit.com)
+ [Blog - www.inframonit.com](https://www.inframonit.com/)
+ [Documentation - docs.inframonit.com](https://docs.inframonit.com/)
+ [Logotyp: logo.inframonit.com](https://logo.inframonit.com/)

+ [LICENSE](LICENSE)



## About inframonit [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/apidsl/examples/edit/main/DOCS/ABOUT.md)


Few examples:
+ Install apidsl project
+ Install letpath package

## Install apidsl examples

```bash
git clone https://github.com/apidsl/example
````

## Install apidsl [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/apidsl/examples/edit/main/DOCS/INSTALL.md)


Install [apidsl](https://github.com/apidsl/bash) project

```bash
git clone https://github.com/apidsl/bash apidsl
````

install dependencies from file: [apifork.txt](apifork.txt)

```bash
./apifork
```

install packages for apidsl from file: [apidsl.txt](apidsl.txt)

```bash
./apidsl.sh install
```


OR

We are working on apidsl folder

```bash
cd apidsl 
````

install packages inside apidsl

```bash
cd apifork
./add https://github.com/letwhois/bash bash letwhois
./add https://github.com/reactphp/dns php reactphp
```



## Start inframonit [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/apidsl/examples/edit/main/DOCS/START.md)




## Test default function

### Show the example functions

```bash
cat ../scripts/example2.txt
```
http("https://www.rezydent.de/").xpath("title");

---

### Check how it works

```bash
./apidsl.sh ../scripts/example2.txt
```
www | Rezydent Podatkowy Niemiec

---

## Test loaded package function

Install [letpath](https://github.com/letpath/bash) package to apidsl project in /apidsl/bash/letpath

```bash
./add.sh https://github.com/letpath/bash bash letpath
```

### Show the example functions
```bash
cd apidsl
```
```bash
cat ../scripts/example7.txt
```
http("https://www.rezydent.de/").letpath.tag("title");
```bash
./apidsl.sh ../scripts/example7.txt
```
check from command
```bash
./apidsl.sh 'http("https://www.rezydent.de/").letpath.tag("title")'
./apidsl.sh 'letpath.tag("title")'
```

get whois data

```bash
./apidsl.sh 'letwhois.ns("softreck.com")'
```


```bash
./apidsl.sh 'letwhois.reverseIp("8.8.8.8")'
```

get ip from domain host

```bash
./apidsl.sh 'letwhois.domainIp("softreck.com")'
```

```bash
./apidsl.sh 'nslookup("softreck.com")'
```

---

### Check how it works
```bash
./apidsl.sh ../scripts/example7.txt
```
www | Rezydent Podatkowy Niemiec
    
---

## Test removing package function

remove [letpath](https://github.com/letpath/bash) package from apidsl project in /apidsl/bash/letpath

```bash
./del.sh bash letpath
```




## Contribution [<span style='font-size:20px;'>&#x270D;</span>](https://github.com/apidsl/examples/edit/main/DOCS/CONTRIBUTION.md)


Install dependencies after created project
```bash
curl https://raw.githubusercontent.com/apifork/bash/main/apifork.sh -o apifork
echo "apifork.txt" > ".apifork"
echo "" > "apifork.txt"
```

### Update documentation

```bash
 ./readme
```

Config project file

The config file: **.apifork** can be another, e.g. **projects.txt**

Just change the first line in  **.apifork** on **projects.txt**
```bash
projects.txt
```


### install

[minsungson/GitHub-cURL: A guide to installing files from GitHub repos in terminal using cURL](https://github.com/minsungson/GitHub-cURL)

```bash
./apifork install
```
OR

```bash
./apifork
```

### update

```bash
./apifork update
```


### remove

```bash
./apifork remove
```



# Tags

+ scripts
+ language

---

+ [edit](https://github.com/apidsl/examples/edit/main/README.md)
+ [apidsl/examples](https://github.com/apidsl/examples)
