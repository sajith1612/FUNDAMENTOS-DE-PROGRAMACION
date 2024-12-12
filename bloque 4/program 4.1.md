# P-1 pop from a list
# Sajith Alexandro Montano Grimaldo
# 04-11-2024

# Lista inicial
lista_num = [10, 30, 40, 20, 35, 80]

# Inicializamos variables para la tabla
i_total = 0  # Suma acumulada de i
print(f"{'Iteración':<10}{'n':<10}{'i':<10}")  # Encabezado de la tabla

# Iteramos a través de la lista y mostramos la tabla
for iteracion, n in enumerate(lista_num, start=1):
    i_total += n
    print(f"{iteracion:<10}{n:<10}{i_total:<10}")
