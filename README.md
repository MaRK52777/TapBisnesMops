<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Мопс</title>
    <style> body { font-family: Arial, sans-serif; text-align: center; background-color: aqua; } 
    h1 { color: blue; font-size: 48px; } .counter { font-size: 2em; margin-top: 50px; }
    button { padding: 30px; border-radius: 50%; font-size: 1.5em; cursor: pointer; border: none; 
    background-color: rgb(150, 18, 173); color: white; } button:hover { background-color: rgb(120, 14, 138); } </style>
</head>
<body>
    <h1>TapMops</h1>
    <div class="counter">
        <img src="34cf4c24-3524-494b-98df-d440b516ce73-Photoroom.png" alt="монета" width="150" height="150">
        : <span id="count">0</span>
    </div>
    <br>
    <button onclick="increment()">
        <img id="dogImage" src="656a1e78-cb1c-4d3c-a2a6-f74d75c6f5f7-Photoroom.png" alt="Кнопка мопса" width="200" height="200">
    </button>
    
    <script>  let count = 0; let clicks = 0; let profitPerTap = 1; 
    function increment() { clicks++; count += profitPerTap; document.getElementById('count').textContent = count;
    if (clicks % 50 == 0 && profitPerTap < 50) { profitPerTap++; alert(`Поздравляем! Вы достигли нового уровня! Теперь ваша прибыль за клик составляет ${profitPerTap} монет.`); 
    if (clicks >= 50) { document.getElementById('dogImage').src = '_im_ad7682cb-22b6-4985-939c-7e3d57094ee9-Photoroom.png'; } } }
   
</script>
</body>
</html>
