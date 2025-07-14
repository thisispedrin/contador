<!DOCTYPE html>
<html>
<Head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>experimento</title>
  <style>
    * {
            margin: 0;
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            background: #010409;
            text-align: center;
            color: black;
            display: grid;
            place-items: center;
        }

        body.white {
            background: rgb(151, 145, 145);
            section {
                background:#ccc ;
            }
            button {
                background: rgb(102, 100, 100);
            }
        }

        button {
            background: rgb(0, 0, 0);
            border-radius: 100px;
            font-size: 40px;
            border-style: none;
            margin: 5px;
            color : rgb(179, 179, 179)
        }

        #zerar:hover {
            scale: 0.95
        }
        button:active {
            scale: 1.3;
        }

        section {
            background: rgb(53, 50, 48);
            padding: 20px;
            border-radius: 20px;
        }

        p {
            font-size: 90px;
        }
        #on_off{

        }</style>
</Head>

<body>
    
    <section>
    <button id="on_off" onclick="on_off()">tema</button>
        <h1>contador</h1>

        <p></p>

        <button onclick="mult()">mult</button>
        <button onclick="aumentar()">mais</button>
        <button id="zerar" onclick="resetar()">zerar</button>
        <button onclick="diminuir()">menos</button>
        <button onclick="divisao()">div</button>
        <button onclick="raiz">porcentagem</button>

    </section>
    
    <script>
        let numero = 0
    
        function on_off(){
            const body = document.querySelector("body")
            body.classList.toggle("white")
            console.log(body)
        }
        function raiz () {
            numero = 50%
            mostrarNatela()
        }

        function aumentar() {
            numero++
            mostrarNatela()
        }
        function divisao() {
            numero /= 2
            mostrarNatela()
        }
        function mult() {
            numero *= 2
            mostrarNatela()
        }
        function diminuir() {
            numero-- 
            mostrarNatela()
        }
        function resetar() {
            numero = 0
            mostrarNatela()
        }
        function mostrarNatela() {
            const p = document.querySelector("p")
            p.innerText = numero
        }

        mostrarNatela()

    </script>
</body>

</html># contador
