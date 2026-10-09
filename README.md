
# PHP Tensor Extension for Windows 

This is the build only version for Windows from RubixML Tensor Ext : https://github.com/RubixML/Tensor-Ext

- click on the version and download the .dlls directly 
- put into your PHP `ext`, and activate in the `php.ini`
	`extension=tensor`
	
- in the local ENV, `libopenblas.dll` is needed. 
	Copy `libopenblas.dll` to the same directory where `php.exe` reside
	For instance if you're using XAMPP copy `libopenblass.dll` to `C:\xampp\php\libopenblas.dll`
  		
- check if loaded and the version 

	```php
	php -r "$ext=get_loaded_extensions();foreach($ext as $x){$item=new ReflectionExtension($x); $v=$item->getVersion(); echo $x.'  '.$v.PHP_EOL;}" | grep tensor
	```

it should return the `tensor` with version, for instance

`tensor  4.1.0`

## version history 

Tensor version	|	PHP Compat	| Build Date 
---------------	|	-----------	| ----
[4.1.0](4.1.0)	|	PHP 8.5	|	09/10/2026 13:56:19
