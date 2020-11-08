## Simple bash passwords generator

# Download code and put code into /usr/local/bin/:
``` sh
git clone https://github.com/RickSunchez/bash_password_generator.git
cd ./bash_password_generator
# copy
cp ./pass /usr/local/bin/
# or move
mv ./pass /usr/local/bin/
# or create symbolic link
ln -s ./pass /usr/local/bin/pass
```

# Or clone this git into /usr/local/bin/:
``` sh
cd /usr/local/bin/
git clone https://github.com/RickSunchez/bash_password_generator.git ./
```

# Examples:
Default:
``` sh
$ pass
#out: ;<Au^($2fjVWYBme
```
You can use next password values:
* -l: password length
* -t: type of using symbols
* -h: help

Param -t using string from 1 to 4 symbols as value. Symbols are:
* d - digits
* a - lowercase alphabet
* A - uppercase alphabet
* s - other symbols

Params examples:
``` sh
$ pass -l 4
#out: 2m1t
$ pass -l 8 -t aA
#out: HAHliyDU
$ pass -l 12 -t s
#out: !}[-#"-.&-,:
$ pass -l 4 -t d
#out: 0176
$ pass -l 32 -t aAds
#out: +v-7&Ha6A+y/kL>{80yk..5tA1G)I33\
```
