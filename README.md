# tareamodificada
def seleccionar_nivel():
    print("Selecciona un nivel de dificultad:")
    print("1. Nivel simple (entre 0 y 100)")
    print("2. Nivel intermedio (entre 0 y 1.000)")
    print("3. Nivel avanzado (entre 0 y 1.000.000)")
    print("4. Nivel experto (entre 0 y 1.000.000.000.000)")
    
    opcion = int(input("Ingresa el número del nivel deseado (1-4): "))
    
    if opcion == 1:
        return 0, 100
    elif opcion == 2:
        return 0, 1000
    elif opcion == 3:
        return 0, 1000000
    elif opcion == 4:
        return 0, 1000000000000
    else:
        print("Opción no válida. Seleccionando nivel simple por defecto.")
        return 0, 100

import random

def generar_numero_secreto(minimo, maximo):
    return random.randint(minimo, maximo)
