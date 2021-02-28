# Sistema-de-Cadastramento---Gabriel-Oliveira
Sistema de Cadastramento - Gabriel Oliveira

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cadastro</title>
    <style>
        body{
            background-color: rgb(115, 115, 185);
        color: white;
        font: normal 20pt;
        }
        h1{
            color: rgb(238, 255, 0);
        }
    </style>
</head>
<body>
    <h1>Sistema de Cadastramento!</h1>
    <h2>Dados do Candidato:</h2>
    <h3>Consulta por Nome:</h3>
    <p>Nome: <input type="text" name="txtname" id="txtname"></p>
    <p>Sobrenome: <input type="text" name="txtsname" id="txtsname"></p>
    <h4>Consulta por Sala de Treinamento:</h4>
    <p>Sala: <input type="number" name="txtnumber" id="txtnumber"></p>
    <p>Área de café: <input type="number" name="txtnumber1" id="txtnumber1"></p>
    <p><input type="button" value="Confirmar!" onclick="calcular()"></p>
    <div id="res">
    </div>
		
<script> 
        function calcular() {
            var txtn = window.document.querySelector('input#txtname')
            var txtsn = window.document.querySelector('input#txtsname')   
            var txtnumber = window.document.querySelector('input#txtnumber')     
            var res = window.document.querySelector('div#res')
            var name = String(txtn.value + " " + txtsn.value)
            var num = Number(txtnumber.value)
            var num1 = Number(txtnumber1.value)
        res.innerHTML = `<p>Seu nome completo é <strong>${name}!</strong></p>
                        <p> Sua sala de treinamento é de número ${num}</p>
                        <p> Sua área de café é a área ${num1}</p>`
            
    } 
   
/*    
Pensei em atribuir uma posição de um vetor "numero" para cada canditado confirmado para dividir este numero tornando ele impar ou par e atribuindo o fato de ser impar ou par para sala 1 ou 2 do treinamento
var n = [0,1,2,3,4,5,6,7,8,9]
var total=n/2;
if(n/2=0){
    alert("Sala 01, área de café 01");
}
if(n/2=1){
    alert("Sala 02, área de café 02");
}
alert(total);
*/
</script>
</body>
</html>
