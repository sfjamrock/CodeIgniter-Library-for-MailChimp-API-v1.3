###CodeIgniter Library for MailChimp API v1.3

####MailChimp API v1.3 The CodeIgniter Way

#####Note

This requires that you have an account with MailChimp, and are able to obtain your [API Key Doc](http://kb.mailchimp.com/article/where-can-i-find-my-api-key/) (or make a new one from the [admin](http://admin.mailchimp.com/account/api)).

#####Installation

* Download and extract.
* Place `MCAPI.php` in the `/application/libraries/` folder of your CodeIgniter project.

#####Usage

To load the library:

```
$config = array(
  'apikey' => '', // Insert your api key
  'secure' => FALSE // Optional (defaults to FALSE)
);
$this->load->library('MCAPI', $config, 'mail_chimp');
```    

Then, to use:

```
$test = $this->mail_chimp->listSubscribe($list_id, $email);
var_dump($test);
```

Call all other methods in this manner.

For full documentation on the MailChimp API, visit the [mailchimp api](http://apidocs.mailchimp.com/api/1.3/)
