**# Programa #7 "El bar"

def mostrar_menu():
    print("Bienvenido al bar. Aquí está el menú:")
    print("1. Cerveza - $5")
    print("2. Vino - $7")
    print("3. Refresco - $2")
    print("4. Agua - $1")
    print("0. Salir")

def calcular_costo(opciones):
    precios = {
        1: 5,  # Cerveza
        2: 7,  # Vino
        3: 2,  # Refresco
        4: 1   # Agua
    }
    total = 0
    for opcion in opciones:
        total += precios.get(opcion, 0)
    return total

if __name__ == "__main__":
    opciones = []
    while True:
        mostrar_menu()
        eleccion = int(input("¿Qué bebida deseas? (Ingresa el número, 0 para salir): "))
        
        if eleccion == 0:
            break
        elif eleccion in [1, 2, 3, 4]:
            opciones.append(eleccion)
            print(f"Has agregado la bebida al pedido.")
        else:
            print("Opción no válida. Por favor, elige una opción del menú.")

    if opciones:
        total = calcular_costo(opciones)
        print(f"\nResumen del pedido: {opciones}")
        print(f"Total a pagar: ${total}")
    else:
        print("\nNo has pedido nada. ¡Hasta luego!")
**
