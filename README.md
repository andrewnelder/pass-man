##Introduction
pass-man is a super-lightweight Python script that can be used to
generate a unique password for every site you visit on the internet.
The beauty of a system like this is you don't have to work too hard to
remember your password.  Just don't change your key once you've set it.

##Requirements
- Python 2.6/2.7
- MacOSX 10.6+

##Installation
Make the script executable:
```
chmod a+x pass-man
```

Then either put the script in your path or append your path with the
project directory.

##Usage
```
Usage: pass-man [-a/d/s] [-m MAXCHARS] -u SITENAME

Options:
  -h, --help            show this help message and exit
  -u SITENAME, --sitename=SITENAME
                        Set the sitename.
  -m MAXCHARS, --maxchars=MAXCHARS
                        Set the max number of characters to use.  Default is
                        15.
  -a, --alphas          Do not use alphas [A-Za-z] in password.
  -d, --digits          Do not use digits [0-9] in password.
  -s, --symbols         Do not use symbols in password.
```

###Example
```
$> pass-man -u yelp.com
kJl]ISTVlAvX+`A
```

##Wish List
- A web interface that can do this conversion remotely.  It can be
  accessed via ssh-key or secure tunnel.
