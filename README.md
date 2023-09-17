<html>
<head>
    <title>Калькулятор выгоды</title>
</head>
<body>
    <h1>Калькулятор выгоды</h1>
    <br>
    <p>Формула: N * 30 * S * (100 - m)/100 - 1990<p>
    <br>
    <label for="n">Количество нереализованной еды (N):</label>
    <input type="number" id="n" placeholder="Введите N">
    <br>
    <label for="s">Средняя стоимость одного блюда (S):</label>
    <input type="number" id="s" placeholder="Введите S">
    <br>
    <label for="m">Процент скидки (m):</label>
    <input type="number" id="m" placeholder="Введите m">
    <br>
    <button onclick="calculate()">Рассчитать выгоду</button>
    <p>ВЫГОДА: <span id="result"></span></p>

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
    </script>
</body>
</html>
