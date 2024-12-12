def operaciones(num1, num2, digitos):
    # Aseguramos que los dígitos sean un número válido para el formato
    formato_division = f"{{:.{digitos}f}}"
    
    suma = num1 + num2
    resta = num1 - num2
    multiplicacion = num1 * num2
    # Usamos el formato para limitar los dígitos en la división
    division = formato_division.format(num1 / num2) if num2 != 0 else "Indefinido (División entre 0)"
    modulo = num1 % num2 if num2 != 0 else "Indefinido (División entre 0)"

    # Imprimimos los resultados
    print(f"Números: num1 = {num1}, num2 = {num2}")
    print(f"Suma: {suma}")
    print(f"Resta: {resta}")
    print(f"Multiplicación: {multiplicacion}")
    print(f"División: {division}")
    print(f"Módulo: {modulo}")
    print("----------------------")

# Función principal con ciclo while
def ciclo_operaciones():
    while True:
        comando = input("Escribe 'salir' para terminar el programa o presiona Enter para continuar: ").strip().lower()
        if comando == "salir":
            print("Programa terminado. ¡Hasta luego!")
            break
        
        # Pedir los datos iniciales
        try:
            num1 = float(input("Ingresa el primer número (num1): "))
            num2 = float(input("Ingresa el segundo número (num2): "))
            digitos = int(input("Ingresa la cantidad de dígitos a mostrar en la división: "))
            repeticiones = int(input("¿Cuántas repeticiones deseas?: "))
            
            for i in range(repeticiones):
                print(f"Iteración {i + 1}:")
                operaciones(num1, num2, digitos)
        except ValueError:
            print("Por favor, ingresa un valor válido.")
        except Exception as e:
            print(f"Ocurrió un error inesperado: {e}")
