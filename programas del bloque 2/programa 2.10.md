# Programa: Verificar si puedes ver una película y si eres mayor de edad

def puede_ver_pelicula(edad, edad_requerida=18):
    if edad >= edad_requerida:
        return True
    return False

def es_mayor_de_edad(edad):
    return edad >= 18

if __name__ == "__main__":
    try:
        edad = int(input("Por favor, ingresa tu edad: "))
        
        if es_mayor_de_edad(edad):
            print("Eres mayor de edad.")
        else:
            print("No eres mayor de edad.")
        
        edad_minima_pelicula = 18  # Edad mínima para ver la película
        if puede_ver_pelicula(edad, edad_minima_pelicula):
            print("Puedes ver la película.")
        else:
            print(f"No puedes ver la película, necesitas tener al menos {edad_minima_pelicula} años.")
    
    except ValueError:
        print("Por favor, ingresa una edad válida.")
