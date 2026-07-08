<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
‹meta name="viewport" content="width=device-width, initial-scale=1.0"> <title> Controle de Notas</title>

<style>
*{
margin: 0; padding:0; box-sizing:border-box;
font-family:Arial, Helvetica, sans-serif;
body‹ background:#f2f2f2;
}
.container}
 width:900px;
margin:40px auto; background:white; padding:30px; border-radius: 10px;
box-shadow:0 0 10px rgba(0,0,0,.2);
}
h1{
text-align:center; margin-bottom:20px;
color:#004080;
}
formulario display:grid;
grid-template-columns: 2fr repeat (4,1 fr) auto; gap: 10px;
margin-bottom:25px;
}
inputt
padding: 10px;
border: 1px solid #ccc; border-radius:5px;
}
button‹ background:#007bff;
color: white;
border none;
border-radius:5px;
cursor:pointer; font-size: 16px;
}
button: hover‹
background:#0056b3;
}
table{
width: 100%;
border-collapse collapse;
}
th{
background:#004080;
color: white;
padding: 12px;
{
td{
text-align:center;
padding: 10px;
border-bottom: 1px solid #ddd;
}
.aprovado{
color:green;
font-weight:bold;
}
.reprovado
color:red;
font-weight bold;
}
</style>
</head>
< body>

<div class="container">
<h1> Controle de Notas dos Alunos</h1>
let n2=parseFloat(document.getElementByld("n2"), value);
let n3=parseFloat(document.getElementByld("n3"). value);
let n4-parseFloat(document.getElementByld("n4") value);

if(nome==™️ | isNaN(n1) | isNaN(n2) || isNaN(n3) || isNaN(n))
alert("Preencha todos os campos.");
return;
}
let media=((n1+n2+n3+n4)/4).toFixed (1);
let situacao=“”; 
let classe””;
if(media>=7){
situacao="Aprovado"; classe="aprovado";
}else{
situacao="Reprovado"; classe="reprovado";
}
let linha=`
<tr>
<td>${nome}</td>
<td>${n1}</td>
<td>${n2}</td>
<td>${n3}<td>
<td>${n4}</td>
<td>${media}</td>
<td class="${classe)">${situacao}</td>
</tr>
document. getElementByld("tabela"). innerHTML += linha;
document.getElementByld(“nome") value=“”;document.getElementByld(“n1").value=“”;
document. getElementByld("n2"). value=“”(document.getElementByld("n3") value=“”;
document.getElementByld("n4").value=“”;
}
</script>
</body^
</html>
