# BasicDB Class for PHP

**Description**: BasicDB is a class to teach and use PDO and OOP, using abstract classes, interfaces and adapters. It simplifies also PDO usage.

Includes:
 - BasicDB Class to simplify PDO
 - Crudable Adapter
 - Add, Edit, Index, View, Delete Adapter methods

Other things to include:

  - **Technology stack**: PHP, Composer, PHPUnit should exits
  - **Things to do**: Complete Doccomments.
  - **Status**:  Very very Alpha [CHANGELOG](CHANGELOG.md).
  - **Links to production or demo instances**
  -  No demo.

## Installation

1. Clone repository
2. Composer Install
3. (Optional) ant build

## Configuration

For testing purposes you should create a test database and add credentials to test files.

## Usage

### Cache System Usage
You can use the ->cache()->all() syntax in your all() or first() queries to use the caching class. If you have a query that you don't want to cache, you can use ->nocache()->all() instead.

Remember to include the BasicDB class and set up your caching settings where you include it.

```
 $config['db'] = [
        'host' => 'localhost',
        'name' => 'dbname',
        'user' => 'root',
        'pass' => '',
        'charset' => 'utf8', 
        'cache_dir' => '_cache/db/', // cache directory
        'ttl' => '60' // cache time
    ];
```

See examples doler.

## How to test the software

build/phpunit

## Known issues

No issues yet

## Getting help

mtkocak@mtkocak.net

Feel free to mail mtkocak@gmail.com 

## Getting involved

You can fork this package.
----

## Open source licensing info
1. [TERMS](TERMS.md)
2. [LICENSE](LICENSE)
----

## Credits and references

I already gave credits above but, you can check;

1. [Tayfun Erbilen](http://www.erbilen.net/)
2. [Midori Kocak](http://www.mtkocak.com/)
3. [Open Source Project Template](https://github.com/cfpb/open-source-project-template)
