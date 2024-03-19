### Backend URLS to block in CloudFlare WAF
```sh
/wp-login.php
/wp-admin/   
/wp-admin/admin-ajax.php
/wp-content/ 
/wp-includes/
/xmlrpc.php

```

```sh
Change Default wp-admin URL
IP Whitelisting for wp-admin
Two-Factor Authentication (2FA)
Strong & Long Password (25-30 characters)
Limit Login Attempts
IP Restriction
Disable Directory Indexing
Disable XML-RPC & XML-RPC Pingback (To avoid  DDoS attacks and Bruteforce attacks)

Disable PHP Error Reporting 
Add the code below to wp-config.php
```sh
error_reporting(0);
```
Disable File Editor (From dashboard>Appearance >editor)
Add the code below to wp-config.php
```sh
define('DISALLOW_FILE_EDIT', true) ;
```
Change Database Table prefix  (Optional)
Add the code below to wp-config.php
```sh
$tablePprefix = 'wp_';
```
```
