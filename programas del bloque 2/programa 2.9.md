# Programa #9 "Costo total de un número de artículos"

def calcular_costo_total(articulos):
    costo_total = 0
    for articulo in articulos:
        precio = articulo['precio']
        cantidad = articulo['cantidad']
        costo_total += precio * cantidad
    return costo_total

if __name__ == "__main__":
    articulos = []

    while True:
        nombre_articulo = input("Introduce el nombre del artículo (o 'salir' para terminar): ")
        if nombre_articulo.lower() == 'salir':
            break
        try:
            precio_articulo = float(input(f"Ingrese el precio de {nombre_articulo}: "))
            cantidad_articulo = int(input(f"Ingrese la cantidad de {nombre_articulo}: "))
            articulos.append({'nombre': nombre_articulo, 'precio': precio_articulo, 'cantidad': cantidad_articulo})
        except ValueError:
            print("Por favor, ingresa un precio y cantidad válidos.")

    costo_total = calcular_costo_total(articulos)

    print("\nCosto total de los artículos:")
    for articulo in articulos:
        print(f"{articulo['cantidad']} x {articulo['nombre']} a ${articulo['precio']:.2f} cada uno.")
    print(f"Costo total: ${costo_total:.2f}")
