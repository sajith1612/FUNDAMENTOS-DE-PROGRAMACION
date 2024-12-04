# Programa #1 "Compuertas NOT"

def compuerta_not(entrada):
    # La compuerta NOT invierte la entrada
    salida = 1 - entrada
    return salida

# Ejemplo de uso
if __name__ == "__main__":
    entrada = int(input("Introduce 0 o 1: "))
    if entrada not in [0, 1]:
        print("Entrada no válida. Por favor, introduce 0 o 1.")
    else:
        salida = compuerta_not(entrada)
        print(f"Entrada: {entrada}, Salida: {salida}")
