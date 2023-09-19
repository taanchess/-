<html>
<head>
    <title>Посчитайте свою выгоду</title>
    <style>
        body {
            background-color: #D9D9D9;
            font-family: 'Montserrat', sans-serif;
        }
        h1 {
            color: #E7410D;
        }
    </style>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Montserrat:regular">
</head>
<body>
    <h1>Посчитайте свою выгоду</h1>
    <br>
    <p>Формула: N * 30 * S * ((100 - m) / 100) - 1990</p>
    <br>
    <label for="n">Количество нереализованной еды в день, в блюдах (N):</label> 
    <input type="number" id="n" placeholder=" Введите m" style="border-radius: 10px;">
    <br>
    <br>
    <label for="s">Средняя стоимость одного блюда, в рублях (S):</label>
    <input type="number" id="n" placeholder=" Введите s" style="border-radius: 10px;">
    <br>
    <br>
    <label for="m">Процент скидки (m):</label>
    <input type="number" id="n" placeholder=" Введите m" style="border-radius: 10px;">
    <br>
    <br>
    <br>
    <button onclick="calculate()" style="width: 214px; height: 41px; border-radius: 30px; background: #E7410D; color: white; font-size: 16px;">Рассчитать выгоду</button>
    <br>
    <br>
    <p>ВЫГОДА: <span id="result"></span></p>

    <br>
    <button onclick="leaveRequest()" style="width: 214px; height: 41px; border-radius: 30px; border: 1px solid #E7410D; background: transparent; color: #E7410D; font-size: 16px;">Оставить заявку</button>


    <script>
        function calculate() {
            // Получаем значения из полей ввода
            var n = parseFloat(document.getElementById("n").value);
            var s = parseFloat(document.getElementById("s").value);
            var m = parseFloat(document.getElementById("m").value);

            // Выполняем расчет по вашей формуле
            var result = n * 30 * s * ((100 - m) / 100) - 1990;

            // Отображаем результат на странице
            document.getElementById("result").textContent = result;
        }

        function leaveRequest() {
            window.location.href = "https://b24-0kqxlb.bitrix24site.ru";
        }
    </script>
</body>
</html>
