<?php

$cSession = curl_init(); 
curl_setopt($cSession,CURLOPT_URL,"http://trac.suveechi.com/api/suveechi1.php?vehno=KA05AG3100");
curl_setopt($cSession,CURLOPT_RETURNTRANSFER,true);
curl_setopt($cSession,CURLOPT_HEADER, false); 
$result=curl_exec($cSession);
curl_close($cSession);
echo $result;
?>
