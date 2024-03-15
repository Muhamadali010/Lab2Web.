```py
Nama  : Muhamad Ali M
Nim   : 312210540
Kelas : TI.22.B2
```

# TUGAS

![image](SS/TUGAS.JPG)

# Memulai PHP”

Buat folder lab2_php_dasar pada root directory web server (d:\xampp\htdocs)

![image](SS/0.JPG)

Kemudian untuk mengakses direktory tersebut pada web server dengan mengakses URL:
http://localhost/lab2_php_dasar/

![image](SS/1.JPG)

# PHP Dasar

Buat file baru dengan nama php_dasar.php pada directory tersebut. Kemudian buat kode seperti
berikut.

```py
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>PHP Dasar</title>
</head>
<body>
<h1>Belajar PHP Dasar</h1>
<?php
echo "Hello World";
?>
</body>
</html>
```

Kemudian untuk mengakses hasilnya melalui URL: http://127.0.0.1/lab2_php_dasar/php_dasar.php
![image](SS/2.JPG)

# Variable PHP

Menambahkan variable pada program.

```py
<?php
$nim = "312210540";
$nama = 'Muhamad Ali M';
echo "NIM : " . $nim . "<br>";
echo "Nama : $nama";
?>
```

![image](SS/3.JPG)

# Predefine Variable $\_GET

```py
<?php
echo 'Selamat Datang ' . $_GET['nama'];
?>
```

# Membuat Form Input

```py
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>PHP Dasar</title>
</head>
<body>
<h2>Form Input</h2>
<form method="post">
<label>Nama: </label>
<input type="text" name="nama">
<input type="submit" value="Kirim">
</form>
<?php
echo 'Selamat Datang ' . $_POST['nama'];
?>
</body>
</html>
```

![image](SS/4.JPG)

### Modul Praktikum Pemrograman Web 2

# Operator

```py
<?php
$gaji = 1000000;
$pajak = 0.1;
$thp = $gaji - ($gaji*$pajak);
echo "Gaji sebelum pajak = Rp. $gaji <br>";
echo "Gaji yang dibawa pulang = Rp. $thp";
?>
```

![image](SS/operator.JPG)

# Kondisi IF

```py
<?php
$nama_hari = date("l");
if ($nama_hari == "Sunday") {
echo "Minggu";
} elseif ($nama_hari == "Monday") {
echo "Senin";
} else {
echo "Selasa";
}
?>
```

![image](SS/Kondisi_IF.JPG)

# Kondisi Switch

```py
<?php
$nama_hari = date("l");
switch ($nama_hari) {
case "Sunday":
echo "Minggu";
break;
case "Monday":
echo "Senin";
break;
case "Tuesday":
echo "Selasa";
break;
default:
echo "Sabtu";
?>
```

# Perulangan for

```py
<?php
echo "Perulangan 1 sampai 10 <br />";
for ($i=1; $i<=10; $i++) {
echo "Perulangan ke: " . $i . '<br />';
}
echo "Perulangan Menurun dari 10 ke 1 <br />";
for ($i=10; $i>=1; $i--) {
echo "Perulangan ke: " . $i . '<br />';
}
?>
```

![image](SS/Perulangan_for.JPG)

# Perulangan while

```py
<?php
echo "Perulangan 1 sampai 10 <br />";
$i=1;
while ($i<=10) {
echo "Perulangan ke: " . $i . '<br />';
$i++;
}
?>
```

![image](SS/Perulangan_while.JPG)

# Perulangan dowhile

```py
<?php
echo "Perulangan 1 sampai 10 <br />";
$i=1;
do {
echo "Perulangan ke: " . $i . '<br />';
$i++;
} while ($i<=10);
?>
```

![image](SS/Perulangan_dowhile.JPG)

==================== SEKIAN & TERIMA KASIH ====================
