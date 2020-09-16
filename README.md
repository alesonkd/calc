<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculadora</title>
</head>
<script>
    function calc(e) {
        var operacao = e.value;
        var n1 = parseFloat(document.getElementById("n1").value);
        var n2 = parseFloat(document.getElementById("n2").value);
        var calculo = eval(n1 + operacao + n2);
        if (!isNaN(calculo)) {
            alert(calculo);
        }
    }
</script>
<body>
                <h1>Calculadora</h1>
                <div class="Calculadora">
                    <span>Digite os numeros:</span><br>
                    <input type="text" size="2" id="n1" placeholder="n1"><br>
                    <input type="text" size="2" id="n2" placeholder="n2"><br><br>
                    <input type="button" value="+" onClick="calc(this)">
                    <input type="button" value="-" onClick="calc(this)">
                    <input type="button" value="*" onClick="calc(this)">
                    <input type="button" value="/" onClick="calc(this)">
            </div>
</body>
</html>
