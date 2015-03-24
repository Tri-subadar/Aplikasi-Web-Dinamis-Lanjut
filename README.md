<html>
<head>
<title>Latihan Bahasa PHP</title>
</head>
<body>
    
    
<?php
//Nama : TRI SUBADAR
//NIM  : 12141388

$Jkolom = 10;
$baris = 1;
//tabel
$data_nama=array("","Fast Five","The Hangover II","Thor","Source Code","I am Number Four","Surke Punch","127 Hours","Rango","The King's Speech","Harry Potter and the dealthly hallows Part2"  );
$data_downloads=array("","9.260.000","8.840.000","8.330.000","7.910.000","7.670.000","7.200.000","6.910.000","6.480.000","6.250.000","6.300.000");
$data_grosess=array("","$626.137.675","$561.464.305","$449.326.618","$123.278.618","$144.500.437","$89.792.502","$60.738.797","$245.155.348","$414.211.549","$1.326.111.219");
echo"<table cellspacing=0 cellpadding=0 bgcolor='#fff' width='900' height='300'><tr style=\"color: #fff;\">
    <td bgcolor='#4F81BD'width='80'>No</td>
    <td bgcolor='#4F81BD'width='570'>Movie</td>
    <td bgcolor='#4F81BD' width='100' style=\"text-align: right;\">downloads</td>
    <td bgcolor='#4F81BD' width='150' style=\"text-align: right; padding-right: 4px;\">grosses</td></tr>";
for($angka=1;$angka<=$Jkolom;$angka++){
    // SelangSeling Warna
    if($baris=="1"){
    echo"<tr border-color=#555555 bgcolor='#d5d5d5'>";
    $baris++;
    }else{
    echo"<tr bgcolor='#fff'>";
    $baris--;
    }
    echo"<td align=center>$angka</td>";
    echo"<td style=\"border-left: 1px solid #d5d5d5; padding-left: 10px;\">$data_nama[$angka]</td>
         <td style=\"text-align: right;border-left: 1px solid #d5d5d5; padding-right: 10px;\">$data_downloads[$angka]</td>
         <td style=\"text-align: right;border-left: 1px solid #d5d5d5; padding-left: 10px; padding-right: 4px;\">$data_grosess[$angka]</td>";
    echo "</tr>";
}
echo"</table>";
?>
    <table bgcolor='#4F81BD' width='900'>
        <tr style="color: #fff;"><td align=left>torrenfreak.com</td></tr> 
    </table>
</body>
</html>
