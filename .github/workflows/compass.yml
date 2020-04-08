<?php
date_default_timezone_set("Asia/Bangkok");

include("config.php");

function cek($url){
    sleep(1);
    $cek = file_get_contents($URL_API."?url=$url");
    if(preg_match("/yes/", $cek)){
        $text = "Silahkan Dibuy Lurrr!!! || ".$url;
        $res = file_get_contents("https://api.telegram.org/bot$BOT_TOKEN/sendMessage?chat_id=$CHAT_ID&text=$text");
        return "$url || Available || ";
    }else{
        return "$url || No ";
    }
}

while(true){
    $list = explode("\n", "https://tokopedia.app.link/GUg7bJsYz3?_p=c11c35dc981c66f0eb038ffeee
https://www.tokopedia.com/sepatucompass

for($i=0; $i<count($list); $i++){
    $cek = cek($list[$i]);
    echo $cek."|| ".date('d-m-Y H:i:s')."\n";
}
}
