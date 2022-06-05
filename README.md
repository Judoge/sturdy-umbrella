# sturdy-umbrella
$imgurl = array(
    'https://blog.zets.cn/usr/themes/handsome/assets/img/sj/1.jpg',
    'https://blog.zets.cn/usr/themes/handsome/assets/img/sj/2.jpg',
    'https://blog.zets.cn/usr/themes/handsome/assets/img/sj/3.jpg',
    'https://blog.zets.cn/usr/themes/handsome/assets/img/sj/4.jpg'
);
//var_dump($imgurl);下面贴输出结果
/* array(4) {
    [0]=>
    string(60) "https://blog.zets.cn/usr/themes/handsome/assets/img/sj/1.jpg"
    [1]=>
    string(60) "https://blog.zets.cn/usr/themes/handsome/assets/img/sj/2.jpg"
    [2]=>
    string(60) "https://blog.zets.cn/usr/themes/handsome/assets/img/sj/3.jpg"
    [3]=>
    string(60) "https://blog.zets.cn/usr/themes/handsome/assets/img/sj/4.jpg"
  }
   */
  //如此一来是不是可以直接
$randimgurl = $imgurl[array_rand($imgurl)];
//echo $randimgurl;
header('location:'.$randimgurl);
