def calcular_tiempo(dias):
    # Constantes
    horas_por_dia = 24
    minutos_por_hora = 60
    dias_por_mes = 30  # Aproximación, ya que los meses pueden variar

    # Cálculos
    horas = dias * horas_por_dia
    minutos = horas * minutos_por_hora
    meses = dias / dias_por_mes

    # Resultados
    print(f"Días ingresados: {dias}")
    print(f"Equivalente en horas: {horas} horas")
    print(f"Equivalente en minutos: {minutos} minutos")
    print(f"Equivalente en meses: {meses:.2f} meses")


# Entrada del usuario
try:
    dias_ingresados = int(input("Ingresa la cantidad de días: "))
    if dias_ingresados > 0:
        calcular_tiempo(dias_ingresados)
    else:
        print("Por favor, ingresa un número mayor que 0.")
except ValueError:
    print("Por favor, ingresa un número válido.")
