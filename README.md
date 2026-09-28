#calculadora-html
#uma calculadora 

#html abaixo
<html>
    <head>
        <title>Calculadora</title>
        <meta charset="utf-8"/>
        <script src="calculadora.js"></script>
        <link rel="stylesheet" href="calculadora.css"/>
    </head>
    <body>
        <div style="padding: 14px; margin: 14px; width: 280px;">
            <h1>Calculadora</h1>
            <p>Essa é a minha nova calculadora</p>
            <div id="entradas">
                <div class="campo">
                    <label for="FatorA">Número A:</label><input id="FatorA" type="number"/>
                </div>
                <div class="campo">
                    <label for="FatorB">Número B:</label><input id="FatorB" type="number"/>
                </div>
            </div>
            <div class="butões">
                <button onclick="soma()">+</button>
                <button onclick="subtracao()">-</button>
                <button onclick="multiplicacao()">*</button>
                <button onclick="divisao()">/</button>
            </div>
            <div>
                Resultado: <span id="resultado"></span>
            </div>
        </div>
    </body>
</html>
#css abaixo
ody {
    background-color: darkslategray;
}
div {
    background-color: white;
}
h1 {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
}
#entradas {
    width: 250px;
    display: flex;
    flex-direction: column;
}
.campo {
    flex-direction: row;
}
.botões {
    width: 250px;
}

button {
    width: 30px;
    padding: 4px;
    margin: 4px;
}
#js abaixo
function soma() {
    const a = document.getElementById("FatorA").value;
    const b = document.getElementById("FatorB").value;

    const soma = parseInt(a) + parseInt(b);
    document.getElementById("resultado").innerText = soma;

}
function subtracao() {
    const a = document.getElementById("FatorA").value;
    const b = document.getElementById("FatorB").value;

    const soma = parseInt(a) - parseInt(b);
    document.getElementById("resultado").innerText = soma;
    
}
function multiplicacao() {
    const a = document.getElementById("FatorA").value;
    const b = document.getElementById("FatorB").value;

    const soma = parseInt(a) * parseInt(b);
    document.getElementById("resultado").innerText = soma;
    
}
function divisao() {
    const a = document.getElementById("FatorA").value;
    const b = document.getElementById("FatorB").value;

    const soma = parseInt(a) / parseInt(b);
    document.getElementById("resultado").innerText = soma;
    
}
