# [examples.apidsl.com](https://examples.apidsl.com/)

Few examples:
+ Install apidsl project
+ Install letpath package

## Install apidsl examples

```bash
git clone https://github.com/apidsl/example
````

## START

Install [apidsl](https://github.com/apidsl/bash) project

```bash
git clone https://github.com/apidsl/bash apidsl
````

We are working on apidsl folder
```bash
cd apidsl 
````

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
cat ../scripts/example7.txt
```
http("https://www.rezydent.de/").letpath.tag("title");

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



## TODO

+ apimacro
+ flatedit
+ Examples with plainedit