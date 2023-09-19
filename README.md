<html>
<head>
    <title>Калькулятор выгоды</title>
    <style>
        body {
            background-color: #D9D9D9; /* Фоновый цвет */
            font-family: 'Montserrat', sans-serif; /* Шрифт Montserrat */
        }
        
        h1 {
            color: #E7410D; /* Цвет текста */
        }

        .container {
            display: flex;
            align-items: center;
        }

        .calculator {
            flex: 1;
        }

        .image-container {
            flex: 1;
            text-align: center;
        }

        img {
            max-width: 100%;
            height: auto;
            cursor: not-allowed; /* Отключает контекстное меню правой кнопки мыши */
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="calculator">
            <h1>Калькулятор выгоды</h1>
            <br>
            <p>Формула: N * 30 * S * ((100 - m) / 100) - 1990</p>
            <br>
            <label for="n">Количество нереализованной еды в день (N):</label>
            <input type="number" id="n" placeholder="Введите N">
            <br>
            <label for="s">Средняя стоимость одного блюда (S):</label>
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
        </div>
        <div class="image-container">
            <!-- Замените ссылку ниже на URL вашей картинки -->
            <img src="https://vk.com/doc357626168_669639367?hash=PFMzl9iFKcbJuQfHfgciiBUup7eYBZq8bjkAA6ZHxvP&dl=OGW8gSHrbGxORplzq4ZWEaRcB0MiGzaWYpD1JNavPJL" alt="Изображение">
        </div>
    </div>

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

    <!-- Добавляем шрифт Montserrat из Google Fonts -->
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Montserrat">
</body>
</html>
