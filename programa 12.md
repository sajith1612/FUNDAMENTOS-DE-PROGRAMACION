def analizar_compuertas_logicas():
    print("Analizando las compuertas lógicas OR y AND\n")

    # Solicitar valores booleanos
    try:
        entrada1 = input("Ingresa el primer valor (True/False): ").strip().capitalize()
        entrada2 = input("Ingresa el segundo valor (True/False): ").strip().capitalize()

        # Convertir las entradas a booleanos
        valor1 = eval(entrada1) if entrada1 in ["True", "False"] else None
        valor2 = eval(entrada2) if entrada2 in ["True", "False"] else None

        # Validar las entradas
        if valor1 is None or valor2 is None:
            print("\nPor favor, ingresa valores válidos (True o False).")
            return

        # Mostrar resultados de las operaciones lógicas
        print("\nResultados de las operaciones lógicas:")
        print(f"{valor1} AND {valor2}: {valor1 and valor2} (Compuerta AND)")
        print(f"{valor1} OR {valor2}: {valor1 or valor2} (Compuerta OR)")

    except Exception as e:
        print("\nOcurrió un error:", str(e))

# Ejecutar la función
if __name__ == "__main__":
    analizar_compuertas_logicas()
