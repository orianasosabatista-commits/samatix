<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<!-- Estilos CSS -->

<style>
    body{
    background-image: url(img/fondo.avif);
    }
</style>
<!-- fin de estilos -->

<body>
    <input type="number" onchange="imc()" id="npeso" placeholder="peso">
    <input type="number" onchange="imc()" id="naltura" placeholder="altura">
    <button onclick="imc()">calcular</button>
    <h2 id="resultado"></h2>

<!-- funcionalidad java script -->
<script type="text/javascript">
        function imc(){
            var p = npeso.value;
            var a = naltura.value;
            var calc = p / (a*a);
            resultado.innerText = calc;
            //console.log("se me llamo");
        }
</script>
<!-- fin de funcionalidad-->
</body>
</html>
