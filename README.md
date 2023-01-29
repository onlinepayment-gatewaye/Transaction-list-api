# Transaction-list-api
The Transaction list API documentation on Github :
#Api url
https://onlinepayment.biz/api/V1/user/list_trachonesh_user
#parameter
email => Required
#Examples
<?php
$merchant_id="Your_merchant_id";
$url = "https://onlinepayment.biz/api/V1/user/list_trachonesh_user";
$method = "POST";
$content = array(
  'email'=>"your_email_account"
);

$ch = curl_init($url);
curl_setopt($ch, CURLOPT_RETURNTRANSFER, TRUE);
curl_setopt($ch, CURLOPT_HEADER, FALSE);
curl_setopt($ch, CURLOPT_POST, TRUE);
curl_setopt($ch, CURLOPT_POSTFIELDS, $content);
$execResult = curl_exec($ch);
curl_close($ch);

echo $execResult;
?>
