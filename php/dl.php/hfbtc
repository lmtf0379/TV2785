<?php

$id = isset($_GET['id']) ? $_GET['id'] : '1';  //新闻1、生活2、财 经3、教育4、故事5、公共6

$url = 'https://app.hfbtc.cn/shows/2/'.$id.'.html';
$data = file_get_contents($url);
preg_match('/source src="(.*?)"/i',$data,$stream);

if (!empty($stream)) {
    $playurl = $stream[1];
    header('Location: ' . $playurl);
}
exit;

?>