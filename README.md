# Educational-tools
/educational-tools
   ├── index.html  (Main page)
   ├── style.css   (Styling)
   ├── script.js   (Interactive logic)
   ├── tools/
   │   ├── unit-converter.html (Unit conversion tool)
   │   ├── calculator.html (Basic calculator)
   ├── images/  (For icons and logos
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Online Educational Tools</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <h1>Educational Tools</h1>
    </header>

    <nav>
        <ul>
            <li><a href="tools/unit-converter.html">Unit Converter</a></li>
            <li><a href="tools/calculator.html">Calculator</a></li>
        </ul>
    </nav>

    <section class="ads">
        <!-- Google AdSense Code Here -->
    </section>

    <footer>
        <p>&copy; 2025 Educational Tools. All Rights Reserved.</p>
    </footer>

</body>
</html>
body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #f4f4f4;
}

header {
    background-color: #007bff;
    color: white;
    padding: 15px;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 10px;
}

nav ul li a {
    text-decoration: none;
    font-weight: bold;
    color: #333;
}

.ads {
    margin: 20px;
    min-height: 100px; /* Space for AdSense */
}

footer {
    margin-top: 20px;
    padding: 10px;
    background: #333;
    color: white;
}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Calculator</title>
    <link rel="stylesheet" href="../style.css">
</head>
<body>

    <header>
        <h1>Simple Calculator</h1>
    </header>

    <div>
        <input type="text" id="display" readonly>
        <br>
        <button onclick="clearDisplay()">C</button>
        <button onclick="appendNumber('1')">1</button>
        <button onclick="appendNumber('2')">2</button>
        <button onclick="appendNumber('+')">+</button>
        <br>
        <button onclick="appendNumber('3')">3</button>
        <button onclick="appendNumber('4')">4</button>
        <button onclick="appendNumber('5')">5</button>
        <button onclick="appendNumber('-')">-</button>
        <br>
        <button onclick="appendNumber('6')">6</button>
        <button onclick="appendNumber('7')">7</button>
        <button onclick="appendNumber('8')">8</button>
        <button onclick="appendNumber('*')">*</button>
        <br>
        <button onclick="appendNumber('9')">9</button>
        <button onclick="appendNumber('0')">0</button>
        <button onclick="calculateResult()">=</button>
        <button onclick="appendNumber('/')">/</button>
    </div>

    <script>
        function appendNumber(num) {
            document.getElementById("display").value += num;
        }

        function clearDisplay() {
            document.getElementById("display").value = "";
        }

        function calculateResult() {
            document.getElementById("display").value = eval(document.getElementById("display").value);
        }
    </script>

</body>
</html>
