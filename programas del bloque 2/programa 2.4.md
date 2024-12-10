# Programa #4 "Calcular los impuestos y dar un valor"

def calcular_impuestos(income, tax_rate):
    # Calcula el monto de impuestos y el ingreso neto
    impuestos = income * tax_rate / 100
    ingreso_neto = income - impuestos
    return impuestos, ingreso_neto

# Ejemplo de uso
if __name__ == "__main__":
    # Solicitar el ingreso y la tasa de impuesto al usuario
    ingreso = float(input("Introduce el ingreso total: "))
    tasa_impuesto = float(input("Introduce la tasa de impuesto en %: "))
    
    # Llamar a la función
    impuestos, ingreso_neto = calcular_impuestos(ingreso, tasa_impuesto)
    
    # Imprimir resultados
    print(f"Monto de impuestos: {impuestos:.2f}")
    print(f"Ingreso neto después de impuestos: {ingreso_neto:.2f}")
