# programa 2 "programa que si chotis y choto van a una fiesta, no hay fiesta"

def verificar_fiestas(chotis, choto):
# verificar si ambos chotis y choto estan presentes
if chotis and choto:
return "no hay fiesta"
else: 
return "la fieta esta en marcha"

# ejemplo de uso
if_name_== "_main_":
chotis= input("esta chotis en la fiesta (si/no):").str().lower() == "si"
choto= input("esta chotis en la fiesta (si/no):").str().lower() == "no"

resultado = varifica_fiesta(chotis, choto)
print(resultado)
