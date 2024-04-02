<?php

// 7175874640:AAHgb4IxqxSoZ74_Bb8TbwDNs2ypndrmd5U

$id = $_REQUEST['id'];
	$token = $_REQUEST['token'];
	$from = $_REQUEST['from'];
	$to = $_REQUEST['to'];
	$text = $_REQUEST['text'];

	if ($token == "[your_token]") {
		echo "Thank you $from for sending $text";
	} else {
		echo "Incorrect token";
		die;

 https://api.telegram.org/bot7175874640:AAHgb4IxqxSoZ74_Bb8TbwDNs2ypndrmd5U/Sendmessage?chat_id=7060003386smsperangkat&text=1
 

 }
