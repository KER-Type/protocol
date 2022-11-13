# Protocol

## Clients messages :

`CONNECTION -->`
Tells the server client wants to connect

`MOVE_PLAYER [ID] [X] [Y] -->`
Tells the server client [ID] wants to move to coordinates [X];[Y]

`SHOOT [ID] -->`
Tells the server client [ID] wants to shoot

`DEAD_MONSTER -->`
Tell the server the monster should be dead

## Server messages :

`<-- ADD_PLAYER [X] [Y]`
Tells ALL clients to add a player at coordinates [X];[Y]

`<-- SET_PLAYER [ID]`
Tells a client which spaceship he's controlling

`<-- MOVE_PLAYER [ID] [X] [Y]`
Tells ALL clients to move spaceship [ID] to coordinates [X];[Y]

`<-- SHOOT [ID]`
Tells ALL clients that spaceship [ID] is shooting

`<-- ADD_MONSTER [NAME] [X] [Y]`
Tells ALL clients to create monster [NAME] on coordinates [X];[Y]
