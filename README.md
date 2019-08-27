## plugin-tracker-php

#PHP

For a PHP plugin or library

Simply import the class-paystack-plugin-tracker.php file into your codebase

** include_once plugin_dir_path(__FILE__) . 'class-paystack-plugin-tracker.php';

Initialize the class with the plugin name, and merchant's public key

 ** $pstk_logger = new paystack_plugin_tracker(PLUGIN_NAME, MERCHANT_PUBLIC_KEY);
 
 Then after verifying a transaction status to be successful, call the *log_transaction_success* method
 
 ** $pstk_logger->log_transaction_success(TRANSACTION_REFERNCE);
 
 Voila!
 
 PS: If this is a Wordpress plugin, you should namespace the class in the class-paystack-plugin-tracker.php file to include your plugin's variable prefix like 
 
 **class pff_paystack_plugin_tracker . . .
