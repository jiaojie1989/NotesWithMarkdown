Install
====
参照[Laravel 5 系列入门教程（一）](http://lvwenhan.com/laravel/432.html)
* 安装php，开启mcrypt扩展
* 安装composer包管理器
```bash
curl -sS https://getcomposer.org/installer | php
```
* 使用命令行安装laravel 5
```bash
composer create-project laravel/laravel learnlaravel5
```
如果顺利的话，安装结果应该如下所示：
```
Installing laravel/laravel (v5.0.1)
  - Installing laravel/laravel (v5.0.1)
    Loading from cache

Created project in laravel-5
Loading composer repositories with package information
Installing dependencies (including require-dev)
  - Installing vlucas/phpdotenv (v1.1.0)
    Downloading: 100%         

  - Installing symfony/var-dumper (v2.6.4)
    Downloading: 100%         

  - Installing symfony/translation (v2.6.4)
    Downloading: 100%         

  - Installing symfony/security-core (v2.6.4)
    Downloading: 100%         

  - Installing symfony/routing (v2.6.4)
    Downloading: 100%         

  - Installing symfony/process (v2.6.4)
    Downloading: 100%         

  - Installing psr/log (1.0.0)
    Downloading: 100%         

  - Installing symfony/debug (v2.6.4)
    Downloading: 100%         

  - Installing symfony/http-foundation (v2.6.4)
    Downloading: 100%         

  - Installing symfony/event-dispatcher (v2.6.4)
    Downloading: 100%         

  - Installing symfony/http-kernel (v2.6.4)
    Downloading: 100%         

  - Installing symfony/finder (v2.6.4)
    Downloading: 100%         

  - Installing symfony/console (v2.6.4)
    Downloading: 100%         

  - Installing swiftmailer/swiftmailer (v5.3.1)
    Downloading: 100%         

  - Installing jakub-onderka/php-console-color (0.1)
    Downloading: 100%         

  - Installing jakub-onderka/php-console-highlighter (v0.3.1)
    Downloading: 100%         

  - Installing dnoegel/php-xdg-base-dir (0.1)
    Downloading: 100%         

  - Installing nikic/php-parser (v1.1.0)
    Downloading: 100%         

  - Installing psy/psysh (v0.4.1)
    Downloading: 100%         

  - Installing nesbot/carbon (1.16.0)
    Downloading: 100%         

  - Installing mtdowling/cron-expression (v1.0.4)
    Downloading: 100%         

  - Installing monolog/monolog (1.13.0)
    Downloading: 100%         

  - Installing league/flysystem (1.0.2)
    Downloading: 100%         

  - Installing jeremeamia/superclosure (2.0.0)
    Downloading: 100%         

  - Installing ircmaxell/password-compat (v1.0.4)
    Downloading: 100%         

  - Installing doctrine/inflector (v1.0.1)
    Downloading: 100%         

  - Installing danielstjules/stringy (1.9.0)
    Downloading: 100%         

  - Installing symfony/filesystem (v2.6.4)
    Downloading: 100%         

  - Installing classpreloader/classpreloader (1.2.0)
    Downloading: 100%         

  - Installing laravel/framework (v5.0.14)
    Downloading: 100%         

  - Installing sebastian/version (1.0.4)
    Downloading: 100%         

  - Installing sebastian/global-state (1.0.0)
    Downloading: 100%         

  - Installing sebastian/recursion-context (1.0.0)
    Downloading: 100%         

  - Installing sebastian/exporter (1.2.0)
    Downloading: 100%         

  - Installing sebastian/environment (1.2.1)
    Downloading: 100%         

  - Installing sebastian/diff (1.2.0)
    Downloading: 100%         

  - Installing sebastian/comparator (1.1.1)
    Downloading: 100%         

  - Installing symfony/yaml (v2.6.4)
    Downloading: 100%         

  - Installing doctrine/instantiator (1.0.4)
    Downloading: 100%         

  - Installing phpdocumentor/reflection-docblock (2.0.4)
    Downloading: 100%         

  - Installing phpspec/prophecy (v1.3.1)
    Downloading: 100%         

  - Installing phpunit/php-text-template (1.2.0)
    Downloading: 100%         

  - Installing phpunit/phpunit-mock-objects (2.3.0)
    Downloading: 100%         

  - Installing phpunit/php-timer (1.0.5)
    Downloading: 100%         

  - Installing phpunit/php-file-iterator (1.3.4)
    Downloading: 100%         

  - Installing phpunit/php-token-stream (1.4.0)
    Downloading: 100%         

  - Installing phpunit/php-code-coverage (2.0.15)
    Downloading: 100%         

  - Installing phpunit/phpunit (4.5.0)
    Downloading: 100%         

  - Installing phpspec/php-diff (v1.0.2)
    Downloading: 100%         

  - Installing phpspec/phpspec (2.1.1)
    Downloading: 100%         

symfony/var-dumper suggests installing ext-symfony_debug ()
symfony/translation suggests installing symfony/config ()
symfony/security-core suggests installing symfony/validator (For using the user password constraint)
symfony/security-core suggests installing symfony/expression-language (For using the expression voter)
symfony/routing suggests installing symfony/config (For using the all-in-one router or any loader)
symfony/routing suggests installing symfony/expression-language (For using expression matching)
symfony/routing suggests installing doctrine/annotations (For using the annotation loader)
symfony/event-dispatcher suggests installing symfony/dependency-injection ()
symfony/http-kernel suggests installing symfony/browser-kit ()
symfony/http-kernel suggests installing symfony/class-loader ()
symfony/http-kernel suggests installing symfony/config ()
symfony/http-kernel suggests installing symfony/dependency-injection ()
psy/psysh suggests installing ext-pdo-sqlite (The doc command requires SQLite to work.)
monolog/monolog suggests installing graylog2/gelf-php (Allow sending log messages to a GrayLog2 server)
monolog/monolog suggests installing raven/raven (Allow sending log messages to a Sentry server)
monolog/monolog suggests installing doctrine/couchdb (Allow sending log messages to a CouchDB server)
monolog/monolog suggests installing ruflin/elastica (Allow sending log messages to an Elastic Search server)
monolog/monolog suggests installing videlalvaro/php-amqplib (Allow sending log messages to an AMQP server using php-amqplib)
monolog/monolog suggests installing ext-amqp (Allow sending log messages to an AMQP server (1.0+ required))
monolog/monolog suggests installing aws/aws-sdk-php (Allow sending log messages to AWS services like DynamoDB)
monolog/monolog suggests installing rollbar/rollbar (Allow sending log messages to Rollbar)
league/flysystem suggests installing predis/predis (Allows you to use Predis for caching)
league/flysystem suggests installing league/flysystem-eventable-filesystem (Allows you to use EventableFilesystem)
league/flysystem suggests installing league/flysystem-rackspace (Allows you to use Rackspace Cloud Files)
league/flysystem suggests installing league/flysystem-copy (Allows you to use Copy.com storage)
league/flysystem suggests installing league/flysystem-azure (Allows you to use Windows Azure Blob storage)
league/flysystem suggests installing league/flysystem-webdav (Allows you to use WebDAV storage)
league/flysystem suggests installing league/flysystem-aws-s3-v2 (Allows you to use S3 storage with AWS SDK v2)
league/flysystem suggests installing league/flysystem-aws-s3-v3 (Allows you to use S3 storage with AWS SDK v3)
league/flysystem suggests installing league/flysystem-dropbox (Allows you to use Dropbox storage)
league/flysystem suggests installing league/flysystem-cached-adapter (Flysystem adapter decorator for metadata caching)
league/flysystem suggests installing league/flysystem-sftp (Allows you to use SFTP server storage via phpseclib)
league/flysystem suggests installing league/flysystem-ziparchive (Allows you to use ZipArchive adapter)
laravel/framework suggests installing aws/aws-sdk-php (Required to use the SQS queue driver (~2.4).)
laravel/framework suggests installing doctrine/dbal (Required to rename columns and drop SQLite columns (~2.4).)
laravel/framework suggests installing guzzlehttp/guzzle (Required to use the Mailgun and Mandrill mail drivers (~5.0).)
laravel/framework suggests installing iron-io/iron_mq (Required to use the iron queue driver (~1.5).)
laravel/framework suggests installing league/flysystem-aws-s3-v2 (Required to use the Flysystem S3 driver (~1.0).)
laravel/framework suggests installing league/flysystem-rackspace (Required to use the Flysystem Rackspace driver (~1.0).)
laravel/framework suggests installing pda/pheanstalk (Required to use the beanstalk queue driver (~3.0).)
laravel/framework suggests installing predis/predis (Required to use the redis cache and queue drivers (~1.0).)
sebastian/global-state suggests installing ext-uopz (*)
phpdocumentor/reflection-docblock suggests installing dflydev/markdown (~1.0)
phpdocumentor/reflection-docblock suggests installing erusev/parsedown (~1.0)
phpunit/phpunit suggests installing phpunit/php-invoker (~1.1)
phpspec/phpspec suggests installing phpspec/nyan-formatters (~1.0 – Adds Nyan formatters)
Writing lock file
Generating autoload files
Generating optimized class loader
Compiling common classes
Compiling views
Application key [D2ERh2yEjlW9Qyg1RY0CI42xN0QUFjIp] set successfully.
```
