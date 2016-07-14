PHP测试代码，结合POSTMAN已经完成测试，发送POST数据，返回对应JSON字段

	<?php
		//遍历非关联数组
	    // foreach ($_POST as $element){ 
	    //   echo "This Site url is $url! <br />"; 
	    // } 

		//遍历关联数组
		// foreach($_POST as $x=>$x_value)
		// {
		// 	echo ". $x . ":" . $x_value;
		// 	echo ",\n";
		// }

		$last = array_pop($_POST);
		//普通处理
		echo "{";
		foreach($_POST as $x=>$x_value)
		{
			echo $x . ":" . $x_value;
			echo ",\n";
		}
		//特殊处理
		echo $x . ":" . $last;
		echo "}";
		
	?>