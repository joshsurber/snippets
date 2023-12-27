
``` php
// quick and dirty, uses HTTP basic auth
// not secure from intercepted packets!
if (!isset($_SERVER['PHP_AUTH_USER']) ||  
	$_SERVER['PHP_AUTH_USER'] != 'josh' ||  
	$_SERVER['PHP_AUTH_PW'] != 'surber'  
) {  
header('WWW-Authenticate: Basic realm="My Realm"');  
header('HTTP/1.0 401 Unauthorized');  
echo 'Text to send if user hits Cancel button';  
exit;  
}
```
