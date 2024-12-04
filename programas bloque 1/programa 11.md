# Programa para analizar operadores de comparación

def analizar_operadores_comparacion():
    print("Analizando operadores de comparación\n")

    # Ingresar valores
    try:
        valor1 = float(input("Ingresa el primer valor: "))
        valor2 = float(input("Ingresa el segundo valor: "))

        # Mostrar resultados de comparación
        print("\nResultados de comparación:")
        print(f"{valor1} == {valor2}: {valor1 == valor2} (Igualdad)")
        print(f"{valor1} != {valor2}: {valor1 != valor2} (Diferente)")
        print(f"{valor1} > {valor2}: {valor1 > valor2} (Mayor que)")
        print(f"{valor1} < {valor2}: {valor1 < valor2} (Menor que)")
        print(f"{valor1} >= {valor2}: {valor1 >= valor2} (Mayor o igual que)")
        print(f"{valor1} <= {valor2}: {valor1 <= valor2} (Menor o igual que)")

    except ValueError:
        print("\nPor favor, ingresa valores válidos (números).")

# Ejecutar el análisis
if __name__ == "__main__":
    analizar_operadores_comparacion()
