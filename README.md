<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Consultanță Tarot - IsthisTarot</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #2e2b3d;
            color: #e0d3d3;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            line-height: 1.6;
            height: 100vh;
        }
        h1, h2 {
            color: #c3a6f9;
        }
        h1 {
            margin-top: 20px;
        }
        .content {
            max-width: 800px;
            padding: 20px;
            text-align: center;
            background-color: rgba(46, 43, 61, 0.8);
            border-radius: 10px;
        }
        .magic-button {
            padding: 10px 20px;
            font-size: 16px;
            background-color: #c3a6f9;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            color: white;
            margin: 20px 0;
        }
        .response {
            margin-top: 15px;
            font-size: 18px;
            font-weight: bold;
            color: #e0d3d3;
        }
        footer {
            margin: 20px 0;
            font-size: 14px;
            color: #c3a6f9;
        }
    </style>
</head>
<body>
    <div class="content">
        <h1>Consultanță Tarot cu IsthisTarot</h1>
        <p>
            Pune o întrebare și apasă butonul pentru a obține un răspuns! 
        </p>
        
        <button class="magic-button" onclick="getResponse()">Întreabă-mă!</button>
        <div class="response" id="response"></div>
        
        <footer>
            &copy; 2023 IsthisTarot. Toate drepturile rezervate.
        </footer>
    </div>

    <script>
        function getResponse() {
            const responses = ["Da", "Nu"];
            const randomResponse = responses[Math.floor(Math.random() * responses.length)];
            document.getElementById("response").innerText = randomResponse;
        }
    </script>
</body>
</html>
