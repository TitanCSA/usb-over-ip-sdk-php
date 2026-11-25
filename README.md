# USB-over-IP-SDK PHP SDK

<!-- simple-start:start -->
Use USB-over-IP-SDK from a PHP app.

**Start here.** Run `composer require titancsa/usb-over-ip-sdk`, then try the short example below. Install the matching Windows driver separately.
<!-- simple-start:end -->

> [!IMPORTANT]
> **Contact TitanCSA**
>
> On [Discord](https://discord.com/app), choose **Friends → Add Friend**, enter **`titancsa`** and send the project name. Ask about commercial licensing, integration or support for this project.

`composer require titancsa/usb-over-ip-sdk`

Windows x64 PHP8.2+; enable FFI extension and `ffi.enable=true`.

```php
require "vendor/autoload.php";
$client=new \TitanCSA\Products\USBoverIPSDK\Client();
try {print_r($client->call("client_status"));} finally {$client->close();}
```

[API and operation schema](docs/API.md). Matching driver installed separately.
