QueryBooks
----

`bk` is a command line tool to search books in local directory by file name.

## Installation

```sh
$ [sudo] npm install -g querybooks
```

## Setup

Before using `bk`, you have to config your books directory. Open the user configuration file `$HOME/.bkconf.json` and add the field `booksdir`. Here is an example:

```json
{
    "booksdir": "/Users/kylqin/Documents/books",
    "bookformats": ["pdf", "epub" ,"mobi"]
}
```

## Usage

Execute following command to get the usage:

```sh
$ bk --help
Usage: bk {-h | --help | -v | --version}
       bk [fuzzy | f | lunr | l | simple | s] searchTerm

Options:
   --help, -h      Show this infomation
   --version, -v   Show version

These are common sub commands used to search books with various search engines:

   fuzzy,  f       Search with fuzzy style
   lunr,   l       Search with lunr.js, a search engine which is like Solr
   simple, s       Search with exact match case insensitively
   collect,c       Collect books from collectfrom directories to booksdir
   <searchTerm>    Same search with both simple and lunr sub commands

Please modify the configuration file `/Users/timber/.bkconf.json` (created it if not
existed), assigning the field `booksdir` the path where your books located.
```

## Screenshots

Note that you can open the book by clicking the blue block with holding Command (for MacOS) or Ctrl ( for Linux) key.
<br/>
<br/>
![](https://github.com/qinxij/querybooks/blob/master/screenshots/bk-screenshots01.png?raw=true)
<br/>
<br/>
![](https://github.com/qinxij/querybooks/blob/master/screenshots/bk-screenshots02.png?raw=true)
<br/>
<br/>
![](https://github.com/qinxij/querybooks/blob/master/screenshots/bk-screenshots03.jpg?raw=true)

## License
MIT