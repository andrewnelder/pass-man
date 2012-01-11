##Introduction
pass-man is a super-lightweight Python script that can be used to
generate a unique password for every site you visit on the internet.
The beauty of a system like this is you don't have to work too hard to
remember your password.  Just don't change your key once you've set it.

##Requirements
- [Python 2.6/2.7](http://www.python.org/)
- [XSel 1.2.0+](http://www.kfish.org/software/xsel/download/) (Linux)
- MacOSX / Linux

##Installation
Make the script executable:
```
chmod a+x pass-man
```

Then either put the script in your path or append your path with the
project directory.

##Usage
```
Usage: pass-man [-a/d/s] [-m MAXCHARS] SITENAME

Options:
  -h, --help            Show this help message and exit.
  -u SITENAME, --sitename=SITENAME
                        Set the sitename.
  -m MAXCHARS, --maxchars=MAXCHARS
                        Set the max number of characters to use.  Default is 15.
  -a, --alphas          Do not use alphas [A-Za-z] in password.
  -d, --digits          Do not use digits [0-9] in password.
  -s, --symbols         Do not use symbols in password.
```

###Example
```
$> pass-man yelp.com
kJl]142VlAvX+`A
```

```
$> pass-man -sa yelp.com
142190891023112
```

```
$> pass-man -d yelp.com
kJl]VlAvX+`A)!@
```

##Wish List
- A web interface that can do this conversion remotely.  It can be
  accessed via ssh-key or secure tunnel.
