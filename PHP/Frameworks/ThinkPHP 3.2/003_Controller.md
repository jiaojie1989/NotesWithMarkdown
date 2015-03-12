Controller
====
#### 控制器写法
控制器类的命名方式是：**控制器名（驼峰法，首字母大写）+Controller**

控制器文件的命名方式是：**类名+class.php（类文件后缀）**

e.g.    我们可以在自动生成的Application/Home/Controller目录下面找到一个 IndexController.class.php 文件，这就是默认的Index控制器文件。

默认的欢迎页面其实就是访问的Home模块下面的Index控制器类的index操作方法 我们修改默认的index操作方法如下：
```php
    namespace Home\Controller;
    use Think\Controller;
    class IndexController extends Controller {
        public function index(){
            echo 'hello,world!';
        }
    }
```

#### 控制器用Action命名
需要在配置文件中增加参数控制**DEFAULT_C_LAYER**
```
'DEFAULT_C_LAYER'=>'Action'
```

写法如下
```php
    namespace Home\Action;
    use Think\Action;
    class IndexAction extends Action{
    }
```