# P-7 agrega un ciclo para este código para indicarle cuantas veces debe realizar las operaciones.
# En cada interacción los números que se pasarán en los argumentos serán el doble que el anterior
# sajith alexandro montaño grimaldo
# 16-11-2024

def operaciones(num1, num2, digitos):
    # Aseguramos que los dígitos sean un número válido para el formato
    formato_division = f"{{:.{digitos}f}}"

    suma = num1 + num2
    resta = num1 - num2
    multiplicacion = num1 * num2
    # Usamos el formato para limitar los dígitos en la división
    division = formato_division.format(num1 / num2) if num2 != 0 else "Indefinido (División entre 0)"
    modulo = num1 % num2 if num2 != 0 else "Indefinido (División entre 0)"

    # Imprimimos los resultados
    print(f'Números: num1 = {num1}, num2 = {num2}')
    print(f'Suma: {suma}')
    print(f'Resta: {resta}')
    print(f'Multiplicación: {multiplicacion}')
    print(f'División: {division}')
    print(f'Módulo: {modulo}')
    print('-------------------------')

# Función principal con ciclo
def ciclo_operaciones(num1, num2, digitos, repeticiones):
    for i in range(repeticiones):
        print(f'Iteración {i + 1}:')
        operaciones(num1, num2, digitos)
        # Doblar los números para la siguiente iteración
        num1 *= 2
        num2 *= 2

# Ejemplo de uso
ciclo_operaciones(10, 3, 2, 5)
