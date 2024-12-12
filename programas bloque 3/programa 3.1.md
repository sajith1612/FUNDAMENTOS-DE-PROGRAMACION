# sajith alexandro montaño grimaldo
# programa Elife



class Elife:
    def __init__(self, nombre, salud, energia, felicidad):
        self.nombre = nombre
        self.salud = salud
        self.energia = energia
        self.felicidad = felicidad

    def mostrar_estado(self):
        print(f"{self.nombre} - Salud: {self.salud}, Energía: {self.energia}, Felicidad: {self.felicidad}")

    def comer(self):
        self.energia += 10
        self.salud += 5
        print(f"{self.nombre} ha comido. Energía y Salud aumentadas.")

    def jugar(self):
        if self.energia >= 10:
            self.energia -= 10
            self.felicidad += 15
            print(f"{self.nombre} ha jugado. Energía disminuida y Felicidad aumentada.")
        else:
            print(f"{self.nombre} está demasiado cansado para jugar.")

    def dormir(self):
        self.energia += 20
        self.salud += 10
        print(f"{self.nombre} ha dormido. Energía y Salud aumentadas.")
