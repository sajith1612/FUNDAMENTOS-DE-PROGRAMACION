# Programa para trabajar con Unicode

def mostrar_codigo_unicode():
    # Pedir al usuario un carácter
    caracter = input("Ingresa un carácter: ")
    if len(caracter) == 1:
        # Mostrar el código Unicode
        codigo = ord(caracter)
        print(f"El carácter '{caracter}' tiene el código Unicode: {codigo}")
    else:
        print("Por favor, ingresa solo un carácter.")

def mostrar_caracter_desde_unicode():
    # Pedir al usuario un código Unicode
    try:
        codigo = int(input("Ingresa un código Unicode (número): "))
        # Mostrar el carácter correspondiente
        caracter = chr(codigo)
        print(f"El código Unicode {codigo} corresponde al carácter: '{caracter}'")
    except ValueError:
        print("Por favor, ingresa un número válido.")
    except OverflowError:
        print("El código Unicode ingresado está fuera de rango.")

# Menú principal
def main():
    print("Programa Unicode")
    print("1. Obtener el código Unicode de un carácter")
    print("2. Obtener el carácter desde un código Unicode")
    print("3. Salir")

    while True:
        opcion = input("\nSelecciona una opción (1-3): ")
        if opcion == "1":
            mostrar_codigo_unicode()
        elif opcion == "2":
            mostrar_caracter_desde_unicode()
        elif opcion == "3":
            print("Saliendo del programa. ¡Adiós!")
            break
        else:
            print("Opción no válida. Por favor, selecciona entre 1 y 3.")

# Ejecutar el programa
if __name__ == "__main__":
    main()
