# 04.10
lekcje w dniu 04.10

<!DOCTYPE html>
<html lang="pl">
  <head>
    <title>trójkąt</title>
  </head>
  <body>
    <script>
      let l1;
      let l2;
      let l3;
      while (isNaN(l1)) {
        l1 = parseInt(prompt("podaj 1 bok:"));
      }
      while (isNaN(l2)) {
        l2 = parseInt(prompt("podaj 2 bok:"));
      }
      while (isNaN(l3)) {
        l3 = parseInt(prompt("podaj 3 bok:"));
      }
      if (l1 + l2 > l3 && l1 + l3 > l2 && l2 + l3 > l1) {
        document.write("można zrobić trójkąt");
        document.write("<br>");
        p = (l1 + l2 + l3) / 2;
        y = p * (p - l1) * (p - l2) * (p - l3);
        x = Math.sqrt(y).toFixed(2);
        document.write(x);
      } else {
        document.write("nie można zrobić trójkąta");
      }
    </script>
  </body>
</html>





<!DOCTYPE html>
<html>
  <head>
    <title>calc</title>
  </head>
  <body>
    <p>
      ------------------tylko kalkulator w funkcji---------------------------
    </p>
    <script>
      function calc(l1, l2, z) {
        switch (z) {
          case "+":
            return l1 + l2;
            break;
          case "-":
            return l1 - l2;
            break;
          case "/":
            return l1 / l2;
            break;
          case "*":
            return l1 * l2;
            break;
          default:
            return "zly operator";
            break;
        }
      }
      let l1;
      let l2;
      let z;
      while (isNaN(l1)) {
        l1 = parseInt(prompt("podaj 1 liczbe:"));
      }
      while (isNaN(l2)) {
        l2 = parseInt(prompt("podaj 2 liczbe:"));
      }
      z = prompt("podaj znak:");
      document.write(calc(l1, l2, z));
    </script>
    <p>-----------------wszystko w funkcji----------------------------------</p>
    <script>
      function calc2() {
        let num1;
        let num2;
        let op;
        while (isNaN(num1)) {
          num1 = parseInt(prompt("(zad 2)podaj 1 liczbe:"));
        }
        while (isNaN(num2)) {
          num2 = parseInt(prompt("(zad 2)podaj 2 liczbe:"));
        }
        op = prompt("(zad 2)podaj znak:");
        switch (op) {
          case "+":
            return num1 + num2;
            break;
          case "-":
            return num1 - num2;
            break;
          case "/":
            return num1 / num2;
            break;
          case "*":
            return num1 * num2;
            break;
          default:
            return "zly operator";
            break;
        }
      }
      document.write(calc2());
    </script>
  </body>
</html>
