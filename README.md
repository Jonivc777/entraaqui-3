<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Carta para Ti ❤️</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffebf0;
            padding: 20px;
        }
        .carta {
            background: white;
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
            max-width: 400px;
            margin: auto;
        }
        h1 {
            color: #d63384;
        }
        p {
            color: #333;
            font-size: 18px;
        }
        .boton {
            display: inline-block;
            margin-top: 15px;
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background-color: #ff4d4d;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            text-decoration: none;
        }
        .oculto {
            display: none;
            margin-top: 20px;
            font-size: 18px;
            color: #d63384;
            font-weight: bold;
            text-align: left;
            padding: 10px;
            background: #fff0f5;
            border-radius: 10px;
        }
        .botones-respuesta {
            margin-top: 20px;
        }
        .boton-respuesta {
            display: inline-block;
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            text-decoration: none;
            margin: 5px;
        }
        .si {
            background-color: #ff4d4d;
        }
        .no {
            background-color: #666;
        }
    </style>
</head>
<body>

    <div class="carta">
        <h1>Para Mi Persona Especial ❤️</h1>
        <p>Haz clic en el botón para ver tu mensaje secreto.</p>
        <button class="boton" onclick="mostrarMensaje()">Ver mensaje 💌</button>
        <div id="mensaje" class="oculto">
            <p>Te amo demasiado, mi amor. Eres la mejor de todas. Quiero que entiendas que, por muy lejos que estemos o las discusiones que tengamos, **nunca cometas el error de pensar que no te amo**, porque amarte significa aceptarte tal y como eres.</p>
            <p>Amar es una palabra muy fuerte, y no dejaré de sentirla ni por los kilómetros que nos separen, ni por las peleas absurdas o importantes que tengamos. Todos tienen problemas, para eso se hizo la solución. Y yo estoy dispuesta a seguir amándote y amarte más a pesar de las mil adversidades.</p>
            <p>Te juro que no cambiaría lo que tenemos por nada ni por nadie, simplemente no valdría la pena. **Eres la única chica que mis ojos miran, y no miran a nadie más.** Te amo como no tienes idea, aún no termino de demostrarte mi amor por completo, en serio **no tienes reemplazo.**</p>
            <p>Se que tienes tantos complejos y no puedo con la idea de que tengas que luchar con todos esos pensamientos en tu mente que te torturan. No te mereces todo eso, mi niña. **Te mereces el amor más lindo y sincero**, y me gustaría poder darte todo eso yo 👉🏽👈🏽.</p>
            <p><strong>Ahora después de eso... ¿Aceptas ser mi San Valentín? ❤️</strong></p>
            
            <div class="botones-respuesta">
                <button class="boton-respuesta si" onclick="alert('¡Sabía que dirías que sí! Te amo demasiado ❤️')">Sí, mil veces sí! 💕</button>
                <button class="boton-respuesta no" onclick="hacerMasGrande()">No 😳</button>
            </div>
        </div>
    </div>

    <script>
        function mostrarMensaje() {
            document.getElementById("mensaje").style.display = "block";
        }

        function hacerMasGrande() {
            let botonSi = document.querySelector(".si");
            let tamañoActual = parseInt(window.getComputedStyle(botonSi).fontSize);
            botonSi.style.fontSize = (tamañoActual + 5) + "px"; // Aumenta el tamaño en 5px cada vez
        }
    </script>

</body>
</html>
