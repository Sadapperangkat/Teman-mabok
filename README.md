<?php

// 7175874640:AAHgb4IxqxSoZ74_Bb8TbwDNs2ypndrmd5U
// -7175874640


$id = $_REQUEST['id'];
	$token = $_REQUEST['token'];
	$from = $_REQUEST['from'];
	$to = $_REQUEST['to'];
	$text = $_REQUEST['text'];

	if ($token == "[your_token]") {
		
  
$url = https://api.telegram.org/bot7175874640:AAHgb4IxqxSoZ74_Bb8TbwDNs2ypndrmd5U/Sendmessage";

$postfields = array(
    'chat_id' => "-7175874640",
    'disable_notification' => "True",
    'parse_mode' => "HTML",
    // 'photo' => 'https://image.flaticon.com/teams/new/1-freepik.jpg',
    'text' => "<b>$text</b>",
);

if (!$curld = curl_init()) {
        exit; 
    }

    curl_setopt($curld, CURLOPT_POST, true);
    curl_setopt($curld, CURLOPT_POSTFIELDS, $postfields);
    curl_setopt($curld, CURLOPT_URL,$url);
    curl_setopt($curld, CURLOPT_RETURNTRANSFER, true);

$output = curl_exec($curld);

curl_close ($curld);
    
  
            echo "Thank you $from for sending $text";
	} else {
		echo "Incorrect token";
		die;

} 

 


?>

