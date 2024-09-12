<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cards with Shadows</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #f0f0f0;
        }
        .container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }
        .card {
            background-color: white;
            padding: 20px;
            border-radius: 10px;
            font-size: 16px;
        }
        /* Card Shadows */
        .card1 { box-shadow: none; }
        .card2 { box-shadow: 5px 5px 15px rgba(1, 0, 0, 0.5); } /* Sombra padrão */
        .card3 { box-shadow: inset 5px 5px 15px rgba(0, 0, 0, 0.3); } /* Sombra inicial (inset) */
        .card4 { box-shadow: 5px 5px 5px rgba(01, 0, 0, 0.5), 8px 8px 18px rgba(0, 0, 0, 0.5), 11px 11px 23px rgba(0, 0, 0, 0.3); } /* Múltiplas sombras */
        .card5 { box-shadow: 0px 5px 20px rgba(0, 0, 0, 0.1); } /* Sombra desfocada */
        .card6 { box-shadow: 0px 0px 10px rgba(255, 0, 0, 0.6); } /* Sombra vermelha */

        /* Card Layout */
        .card:nth-child(3) {
            margin-right: auto;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="card card1">
            <h3>Card 1</h3>
            <p>This is the first card.</p>
        </div>
        <div class="card card2">
            <h3>Card 2</h3>
            <p>Este é o segundo cartão com uma sombra.</p>
        </div>
        <div class="card card3">
            <h3>Cartão 3</h3>
            <p>Esta é a terceira carta com uma sombra inicial.</p>
        </div>
        <div class="card card4">
            <h3>Cartão 4</h3>
            <p>Este é o quarto cartão com múltiplas sombras.</p>
        </div>
        <div class="card card5">
            <h3>Cartão 5</h3>
            <p>Este é o quinto cartão com uma sombra desfocada.</p>
        </div>
        <div class="card card6">
            <h3>Cartão 6</h3>
            <p>Este é o sexto cartão com uma sombra vermelha.</p>
        </div>
    </div>

</body>
</html>
