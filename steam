<?php
    header('content-type: image/png');
    
    $stream = $_GET['stream'];
    
    $json_file = @file_get_contents("http://api.twitch.tv/api/stream/list.json?channel={$stream}");
    $json_array = json_decode($json_file, true);
    
    if (strtolower($json_array[0]['name']) == strtolower("live_user_{$stream}")) {
        echo file_get_contents("http://i.imgur.com/ui8Sx6f.jpg");
    }else{
        echo file_get_contents("http://i.imgur.com/KLQLc7k.jpg");
    }

?>
