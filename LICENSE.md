// GRUPO 
GEMA GUERRERO BRAVO
EVELIN MERA QUINTERO
JOSE DAVID VILELA CELORIO




<!DOCTYPE html>

<html>
    <head>
        <title>Tres en Raya</title>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <script>

            function validarX() {

                var a1 = document.getElementById('a1').value;
                var a2 = document.getElementById('a2').value;
                var a3 = document.getElementById('a3').value;
                var b1 = document.getElementById('b1').value;
                var b2 = document.getElementById('b2').value;
                var b3 = document.getElementById('b3').value;
                var c1 = document.getElementById('c1').value;
                var c2 = document.getElementById('c2').value;
                var c3 = document.getElementById('c3').value;

                if (a1 == "x" && a2 == "x" && a3 == "x") {
                   decirGanoX();
                }
                if (b1 == "x" && b2 == "x" && b3 == "x") {
                    decirGanoX();
                }
                if (c1 == "x" && c2 == "x" && c3 == "x") {
                   decirGanoX();
                }
                if (a1 == "x" && b1 == "x" && c1 == "x") {
                    decirGanoX();
                }
                if (a2 == "x" && b2 == "x" && c2 == "x") {
                    decirGanoX();
                }
                if (a3 == "x" && b3 == "x" && c3 == "x") {
                   decirGanoX();
                }
            }

            function validarO() {

                var a1 = document.getElementById('a1').value;
                var a2 = document.getElementById('a2').value;
                var a3 = document.getElementById('a3').value;
                var b1 = document.getElementById('b1').value;
                var b2 = document.getElementById('b2').value;
                var b3 = document.getElementById('b3').value;
                var c1 = document.getElementById('c1').value;
                var c2 = document.getElementById('c2').value;
                var c3 = document.getElementById('c3').value;
                if (a1 == "o" && a2 == "o" && a3 == "o") {
                    decirGanoO();
                }
                if (b1 == "o" && b2 == "o" && b3 == "o") {
                   decirGanoO();
                }
                if (c1 == "o" && c2 == "o" && c3 == "o") {
                    decirGanoO();
                }
                if (a1 == "o" && b1 == "o" && c1 == "o") {
                    decirGanoO();
                }
                if (a2 == "o" && b2 == "o" && c2 == "o") {
                   decirGanoO();
                }
                if (a3 == "o" && b3 == "o" && c3 == "o") {
                   decirGanoO();
                }
            }
            
            function  decirGanoO(){
                alert("Gana: "+document.getElementById('jo').value  +" con la letra O");
            }
             function  decirGanoX(){
                alert("Gana: "+document.getElementById('jx').value  +" con la letra X");
            }

        </script>
    </head>
    <body>

    <center><h1>Tres en Raya</h1>
        <hr><hr>
        Nombre Jugador X: <input type="text" id="jx" value="" />
        Nombre Jugador O: <input type="text" id="jo" value="" />
        <hr>

        <table border="1" >
            <tr>
                <td><input type="text" id="a1" value="" /></td>
                <td><input type="text" id="b1" value="" /></td>
                <td><input type="text" id="c1" value="" /></td>

            </tr>
            <tr>
                <td><input type="text" id="a2" value="" /></td>
                <td><input type="text" id="b2" value="" /></td>
                <td><input type="text" id="c2" value="" /></td>

            </tr>
            <tr>
                <td><input type="text" id="a3" value="" /></td>
                <td><input type="text" id="b3" value="" /></td>
                <td><input type="text" id="c3" value="" /></td>

            </tr>
        </table>
        <input type="button" value="Validar X" onclick="validarX()" />
        <input type="button" value="Validar O" onclick="validarO()" />
    </center>
</body>
</html>
