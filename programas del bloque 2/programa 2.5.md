# Programa #5 "Comparacion, membership, indexing, metodo de slicing"

def mostrar_comparaciones():
    a = 10
    b = 20
    print(f"Comparación de {a} y {b}:")
    print(f"¿Es {a} mayor que {b}? {'Sí' if a > b else 'No'}")
    print(f"¿Es {a} igual a {b}? {'Sí' if a == b else 'No'}")
    print()

def mostrar_membership():
    lista = [1, 2, 3, 4, 5]
    numero = 3
    print(f"¿Está {numero} en la lista {lista}? {'Sí' if numero in lista else 'No'}")
    print()

def mostrar_indexing_y_slicing():
    cadena = "Hola, mundo!"
    lista = [10, 20, 30, 40, 50]
    
    # Indexación
    print(f"Primer carácter de la cadena: '{cadena[0]}'")
    print(f"Último elemento de la lista: {lista[-1]}")
    
    # Slicing
    print(f"Slicing de la cadena (0:4): '{cadena[0:4]}'")
    print(f"Slicing de la lista (1:4): {lista[1:4]}")
    print()

if __name__ == "__main__":
    print("Demostración de comparación, membership, indexing y slicing:")
    mostrar_comparaciones()
    mostrar_membership()
    mostrar_indexing_y_slicing()
