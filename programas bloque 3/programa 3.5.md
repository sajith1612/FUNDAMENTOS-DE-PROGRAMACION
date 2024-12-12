# sajith alexandro montaño grimaldo
# programa que calcule el nivel de desempeño descrito con su calificacion

# Programa para calcular el nivel de desempeño basado en la calificación

def calcular_desempeno(calificacion):
    if calificacion >= 90:
        return "Excelente"
    elif calificacion >= 80:
        return "Muy Bueno"
    elif calificacion >= 70:
        return "Bueno"
    elif calificacion >= 60:
        return "Satisfactorio"
    else:
        return "Insuficiente"

# Entrada del usuario
calificacion = float(input("Introduce tu calificación: "))

# Calcular nivel de desempeño
desempeno = calcular_desempeno(calificacion)

# Mostrar el resultado
print(f"Con una calificación de {calificacion}, tu nivel de desempeño es: {desempeno}")
