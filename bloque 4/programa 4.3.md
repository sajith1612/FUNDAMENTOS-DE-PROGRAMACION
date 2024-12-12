# P-3 Función rango
# 04-11-2024
# Sajith Alexandro Montano Grimaldo

print("Imprime los valores del 0 al 9")
x = range(10)

# Encabezado de la tabla para el primer rango
print(f"{'Iteración':<12}{'Valor'}")
print('-' * 20)

# Imprimir los valores del rango 0-9
for i, num in enumerate(x, start=1):
    print(f"{i:<12}{num}")

print("\nImprime los valores del 5 al 15")
x1 = range(5, 16)

# Encabezado de la tabla para el segundo rango
print(f"{'Iteración':<12}{'Valor'}")
print('-' * 20)

# Imprimir los valores del rango 5-15
for i, num in enumerate(x1, start=1):
    print(f"{i:<12}{num}")

print("\nImprime los pares del 10 al 20")
x2 = range(10, 21, 2)

# Encabezado de la tabla para el tercer rango
print(f"{'Iteración':<12}{'Valor'}")
print('-' * 20)

# Imprimir los valores del rango de los números pares del 10 al 20
for i, num in enumerate(x2, start=1):
    print(f"{i:<12}{num}")

