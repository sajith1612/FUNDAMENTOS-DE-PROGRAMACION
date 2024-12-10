# Programa #8 "Calificaciones aprobó, reprobó"

def evaluar_calificaciones(calificaciones):
    resultados = {}
    for nombre, calificacion in calificaciones.items():
        if calificacion >= 60:
            resultados[nombre] = "Aprobó"
        else:
            resultados[nombre] = "Reprobó"
    return resultados

if __name__ == "__main__":
    calificaciones = {}
    while True:
        nombre = input("Introduce el nombre del estudiante (o 'salir' para terminar): ")
        if nombre.lower() == 'salir':
            break
        try:
            calificacion = float(input(f"Ingrese la calificación de {nombre}: "))
            calificaciones[nombre] = calificacion
        except ValueError:
            print("Por favor, ingresa una calificación válida.")

    resultados = evaluar_calificaciones(calificaciones)

    print("\nResultados de las calificaciones:")
    for nombre, resultado in resultados.items():
        print(f"{nombre}: {resultado}")
