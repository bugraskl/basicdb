
## Cache System Usage
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

### Example Usage
```
// Caching
$db->from('tbl_blogs')->where('blogStatus', 1)->cache()->all();

// Disable Caching

$db->from('tbl_blogs')->where('blogStatus', 1)->nocache()->all();

```

If you encounter a problem, please contact us at contact@bugra.work
