
``` php
function item($a, $b=FALSE, $c=FALSE) {
    if (is_array($a)) {
        $array  = $a;
        $key    = $b;
        $default= $c;
    } elseif (is_array($b)) {
        $array  = $b;
        $key    = $a;
        $default= $c;
    } else {
        $array  = $_REQUEST;
        $key    = $a;
        $default= $b;
    }
    return isset($array[$key]) ? $array[$key] : $default;
}
```
Return an item from an array. If item isn't set, can return a default value. If array isn't set, use `$_REQUEST`. Array and key can be in either order. 