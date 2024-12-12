# sajith alexandro montaño grimaldo

# Programa de indexación en Python

# Ejemplo con listas
lista = [10, 20, 30, 40, 50]
print("Lista completa:", lista)
print("Primer elemento de la lista:", lista[0])
print("Último elemento de la lista:", lista[-1])
print("Sublista del segundo al cuarto elemento:", lista[1:4])

# Ejemplo con tuplas
tupla = (100, 200, 300, 400, 500)
print("\nTupla completa:", tupla)
print("Primer elemento de la tupla:", tupla[0])
print("Último elemento de la tupla:", tupla[-1])
print("Subtupla del segundo al cuarto elemento:", tupla[1:4])

# Ejemplo con cadenas de texto
cadena = "Hola Mundo"
print("\nCadena completa:", cadena)
print("Primer carácter de la cadena:", cadena[0])
print("Último carácter de la cadena:", cadena[-1])
print("Subcadena del segundo al quinto carácter:", cadena[1:5])

# Acceso a elementos dentro de listas de listas
listas_anidadas = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print("\nListas anidadas:", listas_anidadas)
print("Elemento en la primera lista, primer posición:", listas_anidadas[0][0])
print("Elemento en la segunda lista, tercera posición:", listas_anidadas[1][2])
print("Elemento en la tercera lista, segunda posición:", listas_anidadas[2][1])

# Indexación negativa para acceder a elementos desde el final
print("\nUso de indexación negativa")
print("Último elemento de la lista:", lista[-1])
print("Penúltimo elemento de la lista:", lista[-2])
print("Último carácter de la cadena:", cadena[-1])
print("Penúltimo carácter de la cadena:", cadena[-2])
