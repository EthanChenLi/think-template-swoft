# ThinkTemplate for swoft

基于XML和标签库的编译型模板引擎

#### 基于Thinkphp官方修改

该版本为开发版本，不保证功能长期支持。

### 安装方法
```
composer require ethan-chen-li/think-template-swoft
```

### 使用方法：
```php
	$dir = __DIR__."/../../";
	$config = [
		// 模板文件目录
		'view_path'   => $dir.'/resource/views/',
		// 模板编译缓存目录（可写）
		'cache_path'  => $dir.'/runtime/template/',
		// 模板文件后缀
		'view_suffix' => 'html',
	];
	$template = new Template($config);
	$data=[];
	return $template->fetch("list",$data); 
```
请勿使用assign方法或其他方法，不保证功能正常。
模板标签完美支持。



详细用法参考[开发手册](https://www.kancloud.cn/manual/think-template/content)