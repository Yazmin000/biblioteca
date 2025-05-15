# biblioteca
<?php
include('config.php');
error_reporting(0);
$inventario=$_POST["usuario"];
$pass=$_POST["pass"];
$d=mysqli_query($conexion,"SELECT * FROM usuario WHERE correo='{$usuario}' AND contrasena='{$pass}'");
$d=mysqli_fecht_array($d);
if($d['id'] !=""){
    echo "todo bien";
}else{
    echo "todo mal";
}
