# sajith alexandro montaño grimaldo

def es_primo(numero):
    """Verifica si un número es primo."""
    if numero < 2:
        return False
    for i in range(2, int(numero**0.5) + 1):
        if numero % i == 0:
            return False
    return True

def verificar_numero():
    while True:
        try:
            # Solicitar un número al usuario
            numero = int(input("Ingresa un número entre 10 y 90 (o escribe '0' para salir): "))
            
            # Salir del programa si el usuario ingresa 0
            if numero == 0:
                print("¡Programa terminado!")
                break
            
            # Verificar si el número está en el rango
            if 10 <= numero <= 90:
                if es_primo(numero):
                    print(f"El número {numero} está en el rango de 10 a 90 y es primo.")
                else:
                    print(f"El número {numero} está en el rango de 10 a 90 pero NO es primo.")
            else:
                print("El número está fuera del rango de 10 a 90. Intenta nuevamente.")
        except ValueError:
            print("Por favor, ingresa un número válido.")

# Llamar a la función principal
verificar_numero()
