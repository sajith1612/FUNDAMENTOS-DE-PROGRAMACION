# sajith alexandro montaño grimaldo
def es_primo(numero):
    """Verifica si un número es primo."""
    if numero < 2:
        return False
    for i in range(2, int(numero**0.5) + 1):
        if numero % i == 0:
            return False
    return True

def calcular_primo():
    """Solicita al usuario un número y verifica si es primo."""
    try:
        numero = int(input("Ingresa un número para verificar si es primo (o escribe '0' para salir): "))
        
        if numero == 0:
            print("¡Programa terminado!")
            return
        
        if es_primo(numero):
            print(f"El número {numero} es primo.")
        else:
            print(f"El número {numero} no es primo.")
        
        # Llamada recursiva para verificar otro número
        calcular_primo()
    except ValueError:
        print("Por favor, ingresa un número válido.")
        calcular_primo()

# Llamar a la función principal
calcular_primo()
