
``` php
function wfdhtml($tag, $args = array(), $content = '')
{
    if (is_string($args)) $args = ['class' => $args];
    if (is_array($content)) $content = join($content);

    $result = '<' . $tag;
    foreach ($args as $k => $v) {
        $result .= " $k='$v'";
    }
    if (is_null($content)) return $result . " />\n";
    return "$result>$content</$tag>\n";
}
```