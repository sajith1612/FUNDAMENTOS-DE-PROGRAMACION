import math

# solicita el radio del circulo al usuario
radio = float(input("ingrese el radio del circulo"))

# calcula el perimetro (circunferencia) y el área
perimetro = 2 * math.pi * radio
area = math.pi * (radio ** 2)

# mostrar los resultados
print(f"elperimetro del círculo es: {perimetro: .2f}")
print(f"el área del circulo es: {area:.2f}")
