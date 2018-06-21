CyberSource Secure Acceptance
=============================

## Configuration

To run the examples first create a file `config.php` under directory `payment`

```php
<?php

define('MERCHANT_ID', '<MERCHANT_ID>');
define('PROFILE_ID',  '<PROFILE_ID>');
define('ACCESS_KEY',  '<ACCESS_KEY>');
define('SECRET_KEY',  '<SECRET_KEY>');

// DF TEST: 1snn5n9w, LIVE: k8vif92e 
define('DF_ORG_ID', '1snn5n9w');

// TEST PAYMENT URL
define('PAYMENT_URL', 'https://testsecureacceptance.cybersource.com/pay');

// LIVE PAYMENT URL
// define('PAYMENT_URL', 'https://testsecureacceptance.cybersource.com/pay');

/// INQUIRY TRANSACTION STATUS ///
$rpt_username = '<RPT_USERNAME>';
$rpt_password = '<RPT_PASSWORD>';

// proxy
$proxy        = '<PROXY_HOST:PROXY_PORT>';


// EOF
```

## Test

```
$ cd /path/to/cybersource-sa-php
$ php -t . -S 0.0.0.0:8088
```

### Open URL on Web Browser
http://localhost:8088/payment/


## Reference

- [Secure Acceptance Web/Mobile Quick Start Guide (PDF)](https://github.com/e-payment/cybersource-secure-acceptance/blob/master/doc/Secure_Acceptance_WM_Quick_Start_Guide.pdf)
- [Secure Acceptance Web/Mobile Reference Document (PDF)](https://github.com/e-payment/cybersource-secure-acceptance/blob/master/doc/Secure_Acceptance_WM.pdf)

### White-list IP address

All Secure Acceptance notification messaging will originate from a different range of servers and IP addresses. If you are using any Secure Acceptance services, you must add the following IP address ranges to any whitelist or filtering logic.

```
198.241.162.1 - 198.241.162.254
198.241.168.1 - 198.241.168.254
```

- [White-list IP to receive replies and posts from CyberSource](https://support.cybersource.com/s/article/What-IP-addresses-should-I-add-to-my-white-list-to-receive-replies-and-posts-from-CyberSource)