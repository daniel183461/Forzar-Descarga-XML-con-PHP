//LA URL DEL ARCHIVO DEBE SER CON CONEXION FTP EN POCAS PALABRAS /home/userFTP/carpeta/documento
$nombre_fichero = 'urlArchivo';
$fichero_texto = fopen($nombre_fichero, "r");
$contenido_fichero = fread($fichero_texto, filesize($nombre_fichero));

header('Content-Type: text/xml');
header("Content-Disposition:attachment ; filename=nombrearchivo.xml");
header("Cache-Control: no-store, no-cache, must-revalidate");
header("Cache-Control: post-check=0, pre-check=0", false);
header("Pragma: no-cache");

echo $contenido_fichero;
