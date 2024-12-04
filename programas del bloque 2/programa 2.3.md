def operar_variables(operacion, *args):
    """
    Realiza una operación sobre múltiples variables.
    
    Args:
    operacion (str): Tipo de operación ('suma' o 'concatenacion').
    *args: Variables que se desean operar.
    
    Returns:
    Resultado de la operación.
    """
    if operacion == "suma":
        # Verificamos que todos los elementos sean numéricos
        if all(isinstance(arg, (int, float)) for arg in args):
            return sum(args)
        else:
            return "Error: Todos los elementos deben ser números para realizar la suma."
    elif operacion == "concatenacion":
        # Convertimos todos los elementos a cadenas y los concatenamos
        return "".join(str(arg) for arg in args)
    else:
        return "Error: Operación no válida. Usa 'suma' o 'concatenacion'."

# Ejemplo de uso
resultado_suma = operar_variables("suma", 5, 10, 15)
resultado_concatenacion = operar_variables("concatenacion", "Hola", " ", "Mundo", 2024)

print("Resultado de la suma:", resultado_suma)
print("Resultado de la concatenación:", resultado_concatenacion)
