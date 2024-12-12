# Definir personajes de videojuegos
personajes = {
    "link": {"salud": 120, "fuerza": 15},
    "zelda": {"salud": 100, "fuerza": 12},
    "ganondorf": {"salud": 150, "fuerza": 20},
}

# Función para mostrar la salud de un personaje
def mostrar_salud(nombre):
    if nombre in personajes:
        print(f"Salud de {nombre}: {personajes[nombre]['salud']}")
    else:
        print(f"Personaje {nombre} no encontrado.")

# Función creada por el usuario para atacar a un personaje
def atacar(atacante, objetivo):
    if atacante in personajes and objetivo in personajes:
        personajes[objetivo]["salud"] -= personajes[atacante]["fuerza"]
        print(f"{atacante} atacó a {objetivo}. Salud de {objetivo} ahora es {personajes[objetivo]['salud']}.")
    else:
        print("Atacante u objetivo no encontrado.")

# Compuertas AND, OR, NOT
def compuertas_logicas(a, b):
    print(f"a AND b: {a and b}")
    print(f"a OR b: {a or b}")
    print(f"NOT a: {not a}")

# Ejemplo de ciclo for: mostrar atributos de todos los personajes
def mostrar_todos_los_personajes():
    for personaje in personajes:
        mostrar_salud(personaje)

# Entrada del usuario
while True:
    accion = input("¿Qué acción quieres realizar? (mostrar_salud, atacar, compuertas_logicas, mostrar_todos, salir): ")
    if accion == "salir":
        break
    elif accion == "mostrar_salud":
        nombre = input("Introduce el nombre del personaje: ")
        mostrar_salud(nombre)
    elif accion == "atacar":
        atacante = input("Introduce el nombre del atacante: ")
        objetivo = input("Introduce el nombre del objetivo: ")
        atacar(atacante, objetivo)
    elif accion == "compuertas_logicas":
        a = bool(int(input("Introduce 0 o 1 para a: ")))
        b = bool(int(input("Introduce 0 o 1 para b: ")))
        compuertas_logicas(a, b)
    elif accion == "mostrar_todos":
        mostrar_todos_los_personajes()
    else:
        print("Acción no válida. Inténtalo de nuevo.")



        # personajes = {
    "link": {"salud": 120, "fuerza": 15},
    "zelda": {"salud": 100, "fuerza": 12},
    "ganondorf": {"salud": 150, "fuerza": 20},
}


# def mostrar_salud(nombre):
    if nombre in personajes:
        print(f"Salud de {nombre}: {personajes[nombre]['salud']}")
    else:
        print(f"Personaje {nombre} no encontrado.")

# def atacar(atacante, objetivo):
    if atacante in personajes and objetivo in personajes:
        personajes[objetivo]["salud"] -= personajes[atacante]["fuerza"]
        print(f"{atacante} atacó a {objetivo}. Salud de {objetivo} ahora es {personajes[objetivo]['salud']}.")
    else:
        print("Atacante u objetivo no encontrado.")

#def compuertas_logicas(a, b):
    print(f"a AND b: {a and b}")
    print(f"a OR b: {a or b}")
    print(f"NOT a: {not a}")

# def mostrar_todos_los_personajes():
    for personaje in personajes:
        mostrar_salud(personaje)


# while True:
    accion = input("¿Qué acción quieres realizar? (mostrar_salud, atacar, compuertas_logicas, mostrar_todos, salir): ")
    if accion == "salir":
        break
    elif accion == "mostrar_salud":
        nombre = input("Introduce el nombre del personaje: ")
        mostrar_salud(nombre)
    elif accion == "atacar":
        atacante = input("Introduce el nombre del atacante: ")
        objetivo = input("Introduce el nombre del objetivo: ")
        atacar(atacante, objetivo)
    elif accion == "compuertas_logicas":
        a = bool(int(input("Introduce 0 o 1 para a: ")))
        b = bool(int(input("Introduce 0 o 1 para b: ")))
        compuertas_logicas(a, b)
    elif accion == "mostrar_todos":
        mostrar_todos_los_personajes()
    else:
        print("Acción no válida. Inténtalo de nuevo.")

