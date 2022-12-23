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
