# P-7 agrega un ciclo para este código para indicarle cuántas veces debe realizar las operaciones.
# En cada iteración los números que se pasarán en los argumentos serán el doble que el anterior.
# Sajith Alexandro Montaño Grimaldo
# 16-11-2024

def operaciones(num1, num2, digitos):
    # Aseguramos que los dígitos sean un número válido para el formato
    formato_division = f"{{:.{digitos}f}}"

    suma = num1 + num2
    resta = num1 - num2
    multiplicacion = num1 * num2
    # Usamos el formato para limitar los dígitos en la división
    division = formato_division.format(num1 / num2) if num2 != 0 else "Indef."
    modulo = num1 % num2 if num2 != 0 else "Indef."

    # Retornamos los resultados como una lista
    return [num1, num2, suma, resta, multiplicacion, division, modulo]

# Función principal con ciclo
def ciclo_operaciones(num1, num2, digitos, repeticiones):
    # Encabezado de la tabla
    print(f"{'Iteración':<12}{'num1':<10}{'num2':<10}{'Suma':<10}{'Resta':<10}{'Multiplicación':<15}{'División':<15}{'Módulo':<10}")
    print('-' * 90)
    
    # Iteramos a través del número de repeticiones
    for i in range(repeticiones):
        # Obtenemos los resultados de las operaciones
        resultado = operaciones(num1, num2, digitos)
        
        # Imprimimos la fila correspondiente a la iteración
        print(f"{i + 1:<12}{resultado[0]:<10}{resultado[1]:<10}{resultado[2]:<10}{resultado[3]:<10}{resultado[4]:<15}{resultado[5]:<15}{resultado[6]:<10}")
        
        # Doblar los números para la siguiente iteración
        num1 *= 2
        num2 *= 2

# Ejemplo de uso
ciclo_operaciones(10, 3, 2, 5)

