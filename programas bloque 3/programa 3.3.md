# sajith alexandro  montaño grimaldo
# identificacion de tipos de dato

# Programa de identificación de tipos de datos

def identificar_tipo_dato(dato):
    if isinstance(dato, int):
        print(f"{dato} es un entero.")
    elif isinstance(dato, float):
        print(f"{dato} es un flotante.")
    elif isinstance(dato, str):
        print(f"{dato} es una cadena de texto.")
    elif isinstance(dato, list):
        print(f"{dato} es una lista.")
    elif isinstance(dato, dict):
        print(f"{dato} es un diccionario.")
    elif isinstance(dato, bool):
        print(f"{dato} es un booleano.")
    else:
        print(f"No se pudo identificar el tipo de dato de {dato}.")

# Lista de datos de ejemplo
datos = [42, 3.14, "Hola", [1, 2, 3], {"nombre": "Juan", "edad": 30}, True]

# Identificar el tipo de dato para cada elemento en la lista
for dato in datos:
    identificar_tipo_dato(dato)

