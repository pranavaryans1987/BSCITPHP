# BCA2022-23 CSharp Programs

# 1. Addition Of 2 Numbers in PHP
```
<?php
  if(isset($_POST['txtno1']))
  {
    $no1 = $_REQUEST['txtno1'];
    $no2 = $_REQUEST['txtno2'];
    echo $no1+$no2;
  }
?>
<form action="variblaes.php" method="POST">
    <input type="text" name="txtno1" placeholder="Enter No. 1" required>
    <input type="text" name="txtno2" placeholder="Enter No. 2" required>
    <input type="submit" value="Calculate">
</form>
```
## OUTPUT   

![image](https://user-images.githubusercontent.com/31475304/209304573-435062e6-855d-4e1c-a3f3-7eb1b4ad7046.png)

# 2. Addition Of 2 Numbers in PHP With Bootstrap
```
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.2.3/css/bootstrap.min.css" integrity="sha512-SbiR/eusphKoMVVXysTKG/7VseWii+Y3FdHrt0EpKgpToZeemhqHeZeLWLhJutz/2ut2Vw1uQEj2MbRF+TVBUA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
<?php
  if(isset($_POST['txtno1']))
  {
    $no1 = $_REQUEST['txtno1'];
    $no2 = $_REQUEST['txtno2'];
    $total = $no1+$no2;
  }
?>
<div class="container">
    <form action="variblaes.php" method="POST">
        <input type="text" name="txtno1" class="form-control mt-2 mb-2" placeholder="Enter No. 1" required>
        <input type="text" name="txtno2" class="form-control mb-2" placeholder="Enter No. 2" required>
        <input type="submit" class="btn btn-primary w-100" value="Calculate">
    </form>
</div>
<div class="container">
    <div class="card text-center">
        <div class="h3 text-primary">Total is:<?php if(isset($total)){ echo $total;} ?></div>
    </div>
</div>
```

![image](https://user-images.githubusercontent.com/31475304/209306372-29d99fd9-8d44-482d-ad22-b0187047a17b.png)

# 3. Result Using Conditional Statements
```
<?php
	$m1 = $m2 = $m3 = $total = $per = 0;
	$result = $grade = "----";
	if(isset($_POST['txtm1']))
	{
		$m1 = $_POST['txtm1'];
		$m2 = $_POST['txtm2'];
		$m3 = $_POST['txtm3'];
		$total = $m1 + $m2 + $m3;
		if($m1>=40 && $m2 >=40 && $m3 >=40)
		{
			$per = $total / 3;
			$result = "PASS";
			if($per >=70)
			{
				$grade = "A+";
			}
			else if($per >=60)
			{
				$grade = "A";
			}
			else if($per >=50)
			{
				$grade = "B";
			}
			else
			{
				$grade = "C";
			}
		}
		else
		{
			$per = 0;
			$result = "FAIL";
			$grade = "ATKT";
		}
	}
?>
<form action="global.php" method="POST">
	<input type="number" name="txtm1" required>
	<input type="number" name="txtm2" required>
	<input type="number" name="txtm3" required>
	<input type="submit" value="Result">
</form>
<table width="100%">
	<tr>
		<td>Marks1
		<td>Marks2
		<td>Marks3
		<td>Total
		<td>Per
		<td>Grade
		<td>Result
	<tr>
		<td><?php echo $m1; ?>
		<td><?php echo $m2; ?>
		<td><?php echo $m3; ?>
		<td><?php echo $total; ?>
		<td><?php echo $per; ?>
		<td><?php echo $grade; ?>
		<td><?php echo $result; ?>
</table>
```
![image](https://user-images.githubusercontent.com/31475304/210761764-28e399d1-31f6-46ab-826b-a296a4d2d6ef.png)

# 4. PHP Looping Structures
```
<?php
	//For Loop
	for($i=1;$i<=5;$i++)
	{
		for($j=1;$j<=$i;$j++)
		{
			echo $j;
		}
		echo "<br>";
	}
	
	//While Loop
	$i = 1;
	while($i<=5)
	{
		$j = 1;
		while($j<=$i)
		{
			echo $j;
			$j++;
		}
		echo "<br>";
		$i++;
	}
	
	//Do..While Loop
	$i=1;
	do
	{
		$j=1;
		do
		{
				echo $j;
				$j++;
		}while($j<=$i);
		echo "<br>";
		$i++;
	}while($i<=5);
?>
```
