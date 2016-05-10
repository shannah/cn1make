# cn1make

A utility script that will automatically download the dependencies for a Codename One project.  Typically,
Codename One projects are posted on Github without dependencies to save space and bandwidth.  If you want to build the project
locally you have to download a handful of .jar files before the project will build.  This utility will automatically
download those dependencies for you.

## Requirements

Currently this uses a bash script, so will only run in OSX or linux.  It wouldn't be hard to make a .bat file that will run in Windows.

Other Requirements:

* Git
* Ant

## Installation

~~~~
$ sudo curl -k -L https://github.com/shannah/cn1make/raw/master/cn1make > /tmp/cn1make && sudo mv /tmp/cn1make  /usr/local/bin/cn1make && sudo chmod 0755 /usr/local/bin/cn1make
~~~~

(Note:  If you don't want to do sudo, basically all you have to do is download the [cn1make](cn1make) shell script, put it in your PATH, and make it executable).


## Usage

Let's try it out on a sample project:  [Chrome](https://github.com/codenameone/Chrome).

Setting up this project is now as simple as:

~~~~
$ git clone https://github.com/codenameone/Chrome.git
$ cd Chrome
$ cn1make
~~~~

Now you can open the project in Netbeans and it will should build.

## Contact

[Steve Hannah](http://sjhannah.com)

