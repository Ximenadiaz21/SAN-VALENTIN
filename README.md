# SAN-VALENTIN
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Corazón en HTML</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
            margin: 0;
        }

        /* Estilos del corazón */
        .corazon {
            position: relative;
            width: 100px;
            height: 100px;
            background-color: #ff4d4d;
            transform: rotate(-45deg);
            animation: latido 1.2s infinite;
        }

        .corazon::before,
        .corazon::after {
            content: "";
            position: absolute;
            width: 100px;
            height: 100px;
            background-color: #ff4d4d;
            border-radius: 50%;
        }

        .corazon::before {
            top: -50px;
            left: 0;
        }

        .corazon::after {
            top: 0;
            left: 50px;
        }

        /* Animación de latido */
        @keyframes latido {
            0% { transform: rotate(-45deg) scale(1); }
            20% { transform: rotate(-45deg) scale(1.2); }
            40% { transform: rotate(-45deg) scale(1.1); }
            60% { transform: rotate(-45deg) scale(1.3); }
            100% { transform: rotate(-45deg) scale(1); }
        }
    </style>
</head>
<body>

    <div class="corazon"></div>

</body>
</html>
