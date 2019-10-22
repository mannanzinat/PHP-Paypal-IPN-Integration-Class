# PHP-Paypal-IPN-Integration-Class with error fix "Methods with the same name as their class will not be constructors in a future version of PHP; Paypal has a deprecated constructor"

PHP Paypal IPN Integration Class
PHP Version Support: PHP5.x.x, 7.x.x

<code>
<?php
include("paypal.class.php");
$p = new paypal_class;
$p->ipn_log_file = 'paypal.log';
// testing only -
$p->paypal_url = 'domain.com/cgi-bin/webscr';
if( $p->validate_ipn() ) { }
?></code>
