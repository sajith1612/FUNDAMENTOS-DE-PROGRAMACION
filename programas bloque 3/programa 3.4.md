# sajith alexandro montaño grimaldo
# programa que calcule los impuestos con if, elife,else

# Programa para calcular impuestos basado en el ingreso

def calcular_impuesto(ingreso):
    if ingreso <= 10000:
        tasa = 0.10  # 10% de impuestos para ingresos hasta 10,000
    elif ingreso <= 20000:
        tasa = 0.15  # 15% de impuestos para ingresos entre 10,001 y 20,000
    elif ingreso <= 35000:
        tasa = 0.20  # 20% de impuestos para ingresos entre 20,001 y 35,000
    elif ingreso <= 50000:
        tasa = 0.25  # 25% de impuestos para ingresos entre 35,001 y 50,000
    else:
        tasa = 0.30  # 30% de impuestos para ingresos mayores de 50,000

    impuesto = ingreso * tasa
    return impuesto

# Entrada del usuario
ingreso_anual = float(input("Introduce tu ingreso anual: "))

# Calcular impuestos
impuesto_a_pagar = calcular_impuesto(ingreso_anual)

# Mostrar el resultado
print(f"Para un ingreso anual de {ingreso_anual}, los impuestos a pagar son: {impuesto_a_pagar}")
