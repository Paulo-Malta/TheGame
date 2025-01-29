<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lion</title>

    <style>
        body{
            background-color: darkslategray;
            color: whitesmoke;
            font-family: Arial, Helvetica, sans-serif;
            font-size: 18pt;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
           

        }

        #d1{
            height: 60px;
            width: 60px;
            background-color: whitesmoke;
            border-radius: 7px;
            box-shadow: 5px 5px 10px gray;
            border: 1px solid black;
            position: absolute;
            bottom: 480px;

        }


    </style>
</head>
<body onkeypress="clique()" id="d2">

<div id="d1"></div>

<?php
$vet = 'carlos';
print($vet[0]);
print($vet[1]);




?>







<script>
var d1 = document.getElementById("d1");
var d2 = document.getElementById("d2");

function clique(event) {
    var top = parseInt(d1.style.top) || 0; 
    var left = parseInt(d1.style.left) || 0;

    if (event.key == "w") {
        d1.style.top = (top - 10) + "px"; 
    }
    if (event.key == "s") {
        d1.style.top = (top + 10) + "px"; 
    }
    if (event.key == "a") {
        d1.style.left = (left - 10) + "px"; 
    }
    if (event.key == "d") {
        d1.style.left = (left + 10) + "px"; 
    }
}


document.addEventListener("keydown", clique);
</script>




</body>
</html>
