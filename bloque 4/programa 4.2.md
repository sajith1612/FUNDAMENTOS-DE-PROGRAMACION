# p-2
# Sajith Alexandro Montaño Grimaldo
# 04-11-2024

# Lista de frutas
frutas = ["manzana", "piña", "plátano"]

# Encabezado de la tabla
print(f"{'Iteración':<10}{'Índice':<10}{'Fruta':<15}")

# Iteramos sobre la lista de frutas
for iteracion, fruta in enumerate(frutas, start=1):
    print(f"{iteracion:<10}{iteracion - 1:<10}{fruta:<15}")

