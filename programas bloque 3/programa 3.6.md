# sajith alexandro montaño grimaldo

# Programa para generar listas de secuencias de valores

# Generar una lista de números naturales
def numeros_naturales(n):
    return list(range(1, n+1))

# Generar una lista de números pares
def numeros_pares(n):
    return list(range(2, n+1, 2))

# Generar una lista de números impares
def numeros_impares(n):
    return list(range(1, n+1, 2))

# Generar una lista de secuencia aritmética
def secuencia_aritmetica(a, d, n):
    return [a + d * i for i in range(n)]

# Ejemplos de uso
n = int(input("Introduce el valor de n para las secuencias: "))

naturales = numeros_naturales(n)
pares = numeros_pares(n)
impares = numeros_impares(n)
a = int(input("Introduce el primer término (a) de la secuencia aritmética: "))
d = int(input("Introduce la diferencia común (d) de la secuencia aritmética: "))
arithmetic = secuencia_aritmetica(a, d, n)

# Mostrar los resultados
print(f"Números naturales hasta {n}: {naturales}")
print(f"Números pares hasta {n}: {pares}")
print(f"Números impares hasta {n}: {impares}")
print(f"Secuencia aritmética con a={a}, d={d}, n={n}: {arithmetic}")
