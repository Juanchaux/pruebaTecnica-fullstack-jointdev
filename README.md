# pruebaTecnica-fullstack-jointdev
Acá esta mi solución a la prueba técnica para la clasificación del proyecto linea amiga de jointdev

# PRUEBA TECNICA CLASIFICACION JOINTDEV
# Lenguaje: Python
# Juan Jose Chaux Gallego
# codigo: 1000364085
# correo: juan.chaux@utp.edu.co
# semestre: 4to

# se define una funcion que contiene los condicionales 
# dentro de un ciclo y que recibe como parametro una lista
# "n" que contiene las notas de los casos a evaluear.
def gradingStudents(n):
 # se crea una lista vacia donde se almacenaran las notas ya redondeadas.
    roundedGrades = []
# ciclo con la variable iterativa i que ira recoriendo 
# las posiciones para acceder a evaluar las condiciones para cada valor
    for i in n:
        if i < 38:
            roundedGrades.append(i)
        else:
            nextMultipleOf5 = (i // 5 + 1) * 5
            if nextMultipleOf5 - i < 3:
                roundedGrades.append(nextMultipleOf5)
            else:
                roundedGrades.append(i)
    return roundedGrades

# lista que contiene las notas a evaluar.
n = [73, 67, 38, 33]

# variable que contiene a la funcion para invocar.
roundedGrades = gradingStudents(n)
print("La lista inicial era " + str(n))
print("La nueva lista redondeada es " + str(roundedGrades))

# ¿Por que crees que es importante crear una línea de atención dentro de
#  la página web de la universidad que tenga un enfoque en casos basados 
# en violencia de género?

# R//: pienso que es fundammental que exista un apoyo a una realidad 
# social que se vive hoy en dia, la violencia de genero deja una huella cada vez mas profunda
# dentro de nuestra sociedad asi que me parece que es un proyecto totalmente necesario
# para darle el apoyo y acompañamiento debidon a las personas que se encuentra en esta situacion
