<?php
    $sum = 0;
	$n = 153;	
	$temp = $n;
	$totalDigits = strlen($n);
	
	while($n != 0) {
		$r = $n%10; 
		$sum = $sum+pow($r, $totalDigits);
		$n = floor($n/10); 
	}
	
	if($sum == $temp) {
		echo "$temp is an armstrong number";
	} else {
		echo "$temp is not an armstrong number";
	}

?>
