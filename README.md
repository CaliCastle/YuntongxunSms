# 云通讯 短信Api

```bash
composer require cali/yuntongxun-sms
```

In ```config/app.php```:
```php
Cali\YuntongxunSms\YuntongxunSmsServiceProvider::class,
```

In aliases array:
```php
'SMS' => Cali\YuntongxunSms\Facade\YuntongxunSms::class,
```

```php 
php artisan vendor:publish
```

Write configuration inside of the  ```.env``` file in the root directory.

```php
SMS::sendTemplateMessage($templateId, ['param1','param2'], $phone_number})
```

```php
SMS::voiceVerify('123123','138xxxx')
```
