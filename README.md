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
    <input type="number" id="n" placeholder="Введите N">
    <br>
    <label for="s">Средняя стоимость одного блюда, в рублях (S):</label>
    <input type="number" id="s" placeholder="Введите S">
    <br>
    <label for="m">Процент скидки (m):</label>
    <input type="number" id="m" placeholder="Введите m">
    <br>
    <br>
    <button onclick="calculate()">Рассчитать выгоду</button>
    <br>
    <br>
    <p>ВЫГОДА: <span id="result"></span></p>

    <br>
    <button onclick="leaveRequest()">Оставить заявку</button>

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
