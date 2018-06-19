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

// EOF
```

## Test

```
cd /path/to/folder/php
php -t . -S 0.0.0.0:8088
```

### Open URL on Web Browser
http://localhost:8088/payment/


## Reference

- [Secure Acceptance Web/Mobile Quick Start Guide (PDF)](https://github.com/e-payment/cybersource-secure-acceptance/blob/master/doc/Secure_Acceptance_WM_Quick_Start_Guide.pdf)
- [Secure Acceptance Web/Mobile Reference Document (PDF)](https://github.com/e-payment/cybersource-secure-acceptance/blob/master/doc/Secure_Acceptance_WM.pdf)
