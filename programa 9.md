# Declaración y asignación de variables
nombre = "Juan"         # Variable de tipo string
edad = 25               # Variable de tipo entero
altura = 1.75           # Variable de tipo flotante
es_estudiante = True    # Variable de tipo booleano

# Mostrar los valores de las variables
print("Nombre:", nombre)
print("Edad:", edad)
print("Altura:", altura, "metros")
print("¿Es estudiante?", es_estudiante)

# Operaciones con variables
nueva_edad = edad + 5  # Sumar a la edad
print("\nEn 5 años, la edad será:", nueva_edad)

# Concatenación de cadenas
mensaje = "Hola, " + nombre + ". Tienes " + str(edad) + " años."
print("\nMensaje:", mensaje)

# Uso de variables en condiciones
if es_estudiante:
    print("\nEres un estudiante.")

# Modificar variables
nombre = "Ana"
nueva_edad = 30
print("\nNuevo nombre:", nombre)
print("Nueva edad:", nueva_edad)
