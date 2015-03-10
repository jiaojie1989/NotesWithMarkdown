数据库填充 Seeder
====
* 新建seed文件

目录databases/seeds/下新建PageTableSeeder.php

```php
<?php

use Illuminate\Database\Seeder;
use App\Page;

class PageTableSeeder extends Seeder {

  public function run()
  {
    DB::table('pages')->delete();

    for ($i=0; $i < 10; $i++) {
      Page::create([
        'title'   => 'Title '.$i,
        'slug'    => 'first-page',
        'body'    => 'Body '.$i,
        'user_id' => 1,
      ]);
    }
  }

}
```
* 修改同级目录下的DatabaseSeeder.php文件
```
$this->call('PageTableSeeder');
```
* 生成composer的autoload文件
```bash
composer dump-autoload
```
* artisan命令执行数据填充
```bash
php artisan db:seed
```