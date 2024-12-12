<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Juego de Mapa de Tamaulipas</title>
    <style>
        body {
            background-color: rgb(3, 25, 96); /* Fondo negro */
            color: white; /* Texto blanco para mejor contraste */
        }
        #mapa {
            width: 60%;
            height: 100vh;
            background-image: url('Tamps (2).png');
            background-size: contain;
            background-position: center;
            background-repeat: no-repeat;
            position: relative;
            float: left;
        }
        #mapa2 {
            width: 30%;
            height: 75vh; /* Aumentado en un 50% */
            background-image: url('Municipio Blanco.png');
            background-size: contain;
            background-position: center;
            background-repeat: no-repeat;
            position: relative;
            float: right;
            margin-top: 20px;
        }
        .municipio {
            position: absolute;
            width: 180px; /* Aumentado en un 50% */
            height: 165px; /* Aumentado en un 50% */
            background-color: rgba(0, 0, 0, 0);
            border-radius: 80%;
            cursor: pointer;
        }
        .incorrecto {
            position: absolute;
            width: 100%; /* Abarca todo el mapa */
            height: 100%; /* Abarca todo el mapa */
            background-color: rgba(0, 0, 0, 0);
            cursor: pointer;
        }
        .mensaje-incorrecto, .mensaje-correcto {
            font-size: 3em; /* Aumentado en un 50% */
            font-weight: bold;
            text-align: center;
            width: 100%;
            position: absolute;
            top: 70%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-family: Arial, sans-serif; /* Aplicar Arial */
        }
        .mensaje-incorrecto {
            color: rgb(255, 0, 0); /* Rojo más fuerte para el mensaje incorrecto */
        }
        .mensaje-correcto {
            color: rgb(0, 255, 0); /* Verde fuerte para el mensaje correcto */
        }
        .tacha-incorrecto {
            font-size: 10em; /* Tamaño de la tacha */
            font-weight: bold;
            color: darkred; /* Rojo más fuerte para la tacha */
            position: absolute;
            top: 10%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-family: Arial, sans-serif;
            display: none; /* Ocultar tacha por defecto */
        }
        .palomita-correcto {
            font-size: 10em; /* Tamaño de la palomita */
            font-weight: bold;
            color: green; /* Color verde para la palomita */
            position: absolute;
            top: 10%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-family: Arial, sans-serif;
            display: none; /* Ocultar palomita por defecto */
        }
    </style>
</head>
<body>
    <h1>Encuentra el Municipio de Méndez</h1>
    <div id="mapa">
        <div class="municipio" style="top: 43.2%; left: 49.9%; z-index: 10;" onclick="verificarMunicipio('Méndez')"></div>
        <div class="incorrecto" style="top: 0; left: 0; z-index: 1;" onclick="verificarMunicipio('Incorrecto')"></div>
        <!-- Agrega más municipios aquí -->
    </div>
    <div id="mapa2"></div>
    <p id="mensaje" class="mensaje-correcto"></p>
    <p class="tacha-incorrecto" id="tacha">✖</p> <!-- Tacha de incorrecto -->
    <p class="palomita-correcto" id="palomita">✔</p> <!-- Palomita de correcto -->

    <script>
        function verificarMunicipio(nombre) {
            const mensajeElement = document.getElementById('mensaje');
            const tachaElement = document.getElementById('tacha');
            const palomitaElement = document.getElementById('palomita');
            if (nombre === 'Méndez') {
                mensajeElement.innerText = '¡Correcto! Has encontrado Méndez.';
                mensajeElement.classList.remove('mensaje-incorrecto');
                mensajeElement.classList.add('mensaje-correcto');
                tachaElement.style.display = 'none'; // Ocultar tacha si es correcto
                palomitaElement.style.display = 'block'; // Mostrar palomita si es correcto
            } else {
                mensajeElement.innerText = 'Incorrecto. Gracias por participar.';
                mensajeElement.classList.remove('mensaje-correcto');
                mensajeElement.classList.add('mensaje-incorrecto');
                tachaElement.style.display = 'block'; // Mostrar tacha si es incorrecto
                palomitaElement.style.display = 'none'; // Ocultar palomita si es incorrecto
            }
        }
    </script>
</body>
</html>
