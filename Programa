# ===================================================
#  Piedra, Papel o Tijera
#  v0.1
#
#  by Julia Martínez 08/2020
#  
# ===================================================

import random

# ---------------------------------------------------
#  Definiciones
# ---------------------------------------------------

Tiradas=["Piedra", "Papel", "Tijera"] #Definimos una lista con las 3 opciones de jugadas
eleccion = "" #tirada del jugador
Juego = True

# ---------------------------------------------------
#  Bienvenida al juego
# ---------------------------------------------------

print()
print("¡Hola!")
print("Vamos a jugar a Piedra, Papel o Tijera.")
print("Las reglas son fáciles: Cada vez que ganes ganarás un punto, si pierdes ganaré puntos yo.")
print("Puedes finalizar el juego siempre que quieras escribiendo 'f'")
nombrejugador = input("¿Cómo te llamamos? ")
print("¡Vamos, " + nombrejugador.capitalize() + "!" )
print("")


# ---------------------------------------------------
#  Configuración del juego
# ---------------------------------------------------

def Jugar():
    puntosjugador = 0 #puntos del jugador
    puntosmaquina = 0 #puntos del pc

    while Juego == True:
        mensaje = "" #reseteando la respuesta
        control = "no" #reseteando el control

        #El usuario Tira
        print()
        mensaje = input("Piedra (r), Papel (p) o Tijera (t): ")
        
        #Poniendo las letras con las tiradas
        if mensaje.lower() == "r":
            eleccion = "Piedra"
            control = "OK"
        elif mensaje.lower() == "p":
            eleccion = "Papel"
            control = "OK"
        elif mensaje.lower() == "t":
            eleccion = "Tijera"
            control = "OK"
        elif mensaje.lower() == "f":
            control = "OK"
            print("¡Hasta la próxima!")
            break
        else:
            print("Respuesta no válida. Para finalizar el juego, escribe 'f'")

        #La maquina Tira
        jugada_maquina = random.choice(Tiradas)

        #Imprimiendo tiradas
        if control == "OK":
            print("")
            print("Piedra, papel o tijera... \nUN... \nDOS... \nTRES... \nYA!")
            print("")
            print("Ordenador: " + jugada_maquina)
            print(nombrejugador.capitalize() + ": " + eleccion)

        #Se calcula quién gana y puntos
        if control == "OK":
            if eleccion == "Piedra" and jugada_maquina == "Piedra":
                print("Ha habido un empate")
            elif eleccion == "Papel" and jugada_maquina == "Piedra":
                print("¡Bravo! ¡Has ganado!")
                puntosjugador = puntosjugador + 1
            elif eleccion == "Tijera" and jugada_maquina == "Piedra":
                print("¡Oh, has perdido...!")
                puntosmaquina = puntosmaquina + 1
            elif eleccion == "Piedra" and jugada_maquina == "Tijera":
                print("¡Bravo! ¡Has ganado!")
                puntosjugador = puntosjugador + 1
            elif eleccion == "Papel" and jugada_maquina == "Tijera":
                print("¡Oh, has perdido...!")
                puntosmaquina = puntosmaquina + 1
            elif eleccion == "Tijera" and jugada_maquina == "Tijera":
                print("Ha habido un empate")
            elif eleccion == "Piedra" and jugada_maquina == "Papel":
                print("¡Oh, has perdido...!")
                puntosmaquina = + 1
            elif eleccion == "Papel" and jugada_maquina == "Papel":
                print("Ha habido un empate")
            elif eleccion == "Tijera" and jugada_maquina == "Papel":
                print("¡Bravo! ¡Has ganado!")
                puntosjugador = puntosjugador + 1
            else:
                print("Si quieres finalizar el juego, escribe 'f'")
            print("")
            print()

        #imprimiendo los puntos, si los hay
        if puntosjugador >= 1 or puntosmaquina >= 1:
            print("-----")
            print("Marcador:")
            print(nombrejugador.capitalize() + ": " + str(puntosjugador))
            print("Ordenador: " + str(puntosmaquina))
            print("")

Jugar()
