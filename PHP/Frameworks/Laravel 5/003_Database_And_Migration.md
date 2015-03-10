Database Migration
====
* 增加数据库用户和权限
```sql
create database laravel5;
grant all privileges on laravel5.* to "laravel5"@"%" identified by "laravel5";
flush privileges;
```
* 修改文件 .env
```
DB_HOST=localhost
DB_DATABASE=laravel5
DB_USERNAME=laravel5
DB_PASSWORD=laravel5
```
* 建立Model
```
php artisan make:model Article
php artisan make:model Page
```
* 修改Model文件

位于databases/migrations/下面

具体参见Illuminate\Database\Schema\Blueprint

```php
Schema::create('articles', function(Blueprint $table)
{
	$table->increments('id');
	$table->string('title');
	$table->string('slug')->nullable();
	$table->text('body')->nullable();
	$table->string('image')->nullable();
	$table->integer('user_id');
	$table->timestamps();
});
```
* 执行建表命令
```
php artisan migrate
```
