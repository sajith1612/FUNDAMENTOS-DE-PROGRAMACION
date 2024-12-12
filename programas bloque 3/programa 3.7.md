# sajith alexandro montaño grimaldo

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lista de Elementos</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        ul {
            list-style-type: none;
        }
        li {
            margin: 5px 0;
        }
    </style>
</head>
<body>
    <h1>Listas de Elementos</h1>
    <h2>Lista de Cadenas de Texto</h2>
    <ul id="lista-cadenas"></ul>

    <h2>Lista de Números Enteros</h2>
    <ul id="lista-enteros"></ul>

    <h2>Lista de Valores Booleanos</h2>
    <ul id="lista-booleanos"></ul>

    <script>
        // Lista de cadenas de texto
        const cadenas = ["Hola", "Mundo", "JavaScript"];
        const listaCadenas = document.getElementById('lista-cadenas');
        cadenas.forEach(cadena => {
            let li = document.createElement('li');
            li.textContent = cadena;
            listaCadenas.appendChild(li);
        });

        // Lista de números enteros
        const enteros = [1, 42, 2024];
        const listaEnteros = document.getElementById('lista-enteros');
        enteros.forEach(entero => {
            let li = document.createElement('li');
            li.textContent = entero;
            listaEnteros.appendChild(li);
        });

        // Lista de valores booleanos
        const booleanos = [true, false, true];
        const listaBooleanos = document.getElementById('lista-booleanos');
        booleanos.forEach(booleano => {
            let li = document.createElement('li');
            li.textContent = booleano;
            listaBooleanos.appendChild(li);
        });
    </script>
</body>
</html>
