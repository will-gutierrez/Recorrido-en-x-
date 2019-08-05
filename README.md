# Recorrido-en-x-
Función para que Reeborg dibuje una equis con estrellas en un mundo de 5x5
'''Define una función para que Reeborg dibuje 
una equis con estrellas en un mundo de 5x5.
Pre: Reeborg está en la posición (1,1),
tiene 9 estrellas y mira al Este.
Pos: Reeborg está en la posición 
(1,1) y mira al Este.'''
def walk():
    put("star")
    repeat 4:
        move()
        turn_left()
        move()
        put("star")
        repeat 3:
            turn_left()
        if wall_in_front():
            repeat 2:
                turn_left()
            repeat 4:
                move()
            put("star")
        if wall_in_front():
            turn_left()
            move()
            turn_left()
            move()
            put("star")
            move()
            move()
            repeat 3:
                turn_left()
            move()
            move()
            put("star")
            turn_left()
            move()
            repeat 3:
                turn_left()
            move()
            put("star")
            repeat 3:
                turn_left()
            repeat 4:
                move()
            repeat 2:
                turn_left()
walk()
