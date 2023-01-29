# Transaction-list-api
The Transaction list API documentation on Github :
# Api url
https://onlinepayment.biz/api/V1/user/list_trachonesh_user
# parameter
email => Required
<br>
*noice : <b>The email you use to log into your account</b>

# Examples
<code>

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

</code>

# Errors
<table>
  <tr>
    <th>Status</th>
    <th>message</th>
  </tr>
  <tr>
    <td>200</td>
    <td>Show Json Data</td>
  </tr>
   <tr>
    <td>404</td>
    <td>Enter email</td>
  </tr>
</table>
