# Programa #6 "Word = hamster"

def analizar_palabra(palabra):
    # Contar la longitud de la palabra
    longitud = len(palabra)

    # Contar las vocales
    vocales = 'aeiou'
    contador_vocales = sum(1 for letra in palabra if letra.lower() in vocales)

    # Buscar una subcadena
    subcadena = "ham"
    existe_subcadena = subcadena in palabra

    return longitud, contador_vocales, existe_subcadena

if __name__ == "__main__":
    palabra = "hamster"

    longitud, contador_vocales, existe_subcadena = analizar_palabra(palabra)

    print(f"Palabra: {palabra}")
    print(f"Longitud: {longitud}")
    print(f"Número de vocales: {contador_vocales}")
    print(f"¿Contiene la subcadena 'ham'? {'Sí' if existe_subcadena else 'No'}")
