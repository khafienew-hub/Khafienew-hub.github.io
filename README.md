<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Halaman Simple Keren</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(135deg, #ff7e5f, #feb47b);
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
        }
        
        .container {
            text-align: center;
            padding: 20px;
            border-radius: 10px;
            background: rgba(0, 0, 0, 0.5);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
        }

        h1 {
            font-size: 3rem;
            margin: 0;
            animation: fadeIn 2s ease-in-out;
        }

        p {
            font-size: 1.25rem;
            margin: 10px 0;
            animation: fadeIn 3s ease-in-out;
        }

        button {
            padding: 10px 20px;
            background-color: #ff7e5f;
            color: white;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #feb47b;
        }

        @keyframes fadeIn {
            0% {
                opacity: 0;
                transform: translateY(-20px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Selamat datang!</h1>
        <p>Ini adalah halaman simple tapi keren. Semoga kamu suka!</p>
        <button onclick="changeMessage()">Klik Saya</button>
    </div>

    <script>
        function changeMessage() {
            const message = document.querySelector('p');
            message.textContent = "Terima kasih telah mengklik! Semoga hari kamu menyenankan!";
        }
    </script>
</body>
</html>
