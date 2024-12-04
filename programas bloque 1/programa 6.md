# Solicitar la base y la altura del triángulo al usuario
base = float(input("Ingrese la base del triángulo: "))
altura = float(input("Ingrese la altura del triángulo: "))

# Calcular el área como flotante
area = (base * altura) / 2.0  # Se puede usar 2.0 para enfatizar que es flotante

# Mostrar el resultado
print(f"El área del triángulo es: {area:.2f}")  # Mostrar con dos decimales
