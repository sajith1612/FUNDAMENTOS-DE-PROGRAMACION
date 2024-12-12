# sajith alexandro montaño grimaldo
# programa 2 comparacion de numeros enteros

# Programa de comparación de números enteros

def comparar_numeros(a, b):
    if a > b:
        print(f"{a} es mayor que {b}")
    elif a < b:
        print(f"{a} es menor que {b}")
    else:
        print(f"{a} es igual a {b}")

# Entrada del usuario
num1 = int(input("Introduce el primer número: "))
num2 = int(input("Introduce el segundo número: "))

# Comparar los números
comparar_numeros(num1, num2)
