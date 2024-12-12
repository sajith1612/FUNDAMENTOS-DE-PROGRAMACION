# p-6
# crear una función dentro de un programa que imprima
# las siguientes operaciones: suma, resta, división, multiplicación, modulo.
# la definición de la función debe de tener 3 parámetros (num1, num2, dígitos) donde "dígitos"
# será la cantidad de dígitos a mostrar después del punto en la operación de división.
# La impresión. print(f'texto {val}')
#
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
    print(f'Suma: {suma}')
    print(f'Resta: {resta}')
    print(f'Multiplicación: {multiplicacion}')
    print(f'División: {division}')
    print(f'Módulo: {modulo}')

# Ejemplo de uso:
operaciones(10, 3, 2)
