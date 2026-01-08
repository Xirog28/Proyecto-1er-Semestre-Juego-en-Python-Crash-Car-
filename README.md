# Proyecto 1er Semestre Juego en Python Crash Car 
El juego titulado “Crash car “retará a un jugador por una carrera  con obstáculos desarollado desde la logica de programacion.


## 📌 Descripción

Analizaremos el problema y de esto obtendremos el algoritmo 
en código en python que será nuestra base para la construcción 
del juego. 
“Crash cars" será un juego de programación enfocado en 
la simulación de una carrera de autos donde el objetivo principal 
es hacer tu mejor “marca” o puntuación, básicamente se puede 
tomar como un bucle infinito.El juego busca que los jugadores 
puedan obtener la habilidad para poder esquivar todos los autos 
(Rectángulos rojos). El participante iniciara el juego con una 
velocidad media baja, mientras recorre la pista ira evadiendo 
autos en su camino para evitar perder. Durante el recorrido, el 
carro ira atravesando autos que llegaran de manera aleatoria que 
según el jugador vaya avanzando con su auto, tantos los autos 
como la velocidad en la pista se ira aumentado. 
Cada vez que el auto choque con otro se perderá la vida 
y automáticamente la carrera se acabará reiniciando el juego. 
Durante la carrera mientras avanza la auto ira acelerando y los 
obstáculos se presentarán con más frecuencias, según se acerque 
el jugador a la meta  
En caso de que el jugador no choque con algún auto será 
su agilidad y rapidez el requisito para que llegue primero a la 
meta y gane. El reto radica en controlar el auto para evitar 
obstáculos, administrar correctamente las vidas y llegar a la 
meta.

## 🛠️ Tecnologías
- Python
- Interfaz Tkinter


## 📚 Conceptos aplicados
- Lógica de programación
- Condicionales y ciclos


## 🚀 Cómo ejecutarlo

Al inicio del juego se le presentará un menú al usuario 
este decidirá si iniciar el juego, ver las reglas y como se mueve, 
por último, tendrá la opción de salir del juego si así lo desea. 
Dentro de las interacciones del juego el usuario deberá 
presionar teclas como las flechas en sentido izquierdo y derecho 
esto será clave para darle dirección al auto y así evitar futuros 
obstáculos.  
Los autos en la pista y/o obstáculos irán apareciendo de 
manera aleatoria y con más frecuencia según el jugador vaya 
acercándose a la meta. Aumentado el flujo de autos, la velocidad 
en la pista y la agilidad del jugador.  
Un contador en la pantalla le ira mostrando al jugador su 
puntaje, con esto el jugador sabrá que cuanto le falta por llegar a 
la meta (cuanto puntaje ha recolectado) y probablemente con qué 
frecuencia acelera la pista.  


## *️⃣ Estructura Logica 

- Métodos en clases: 
Están definidas como el personaje que será nuestro auto y los 
obstáculos que serán los otros autos que impedirán que el 
jugador llegue a la meta.  
La clase “Personaje” representa el auto controlado por el jugador 
definiéndolo de esta manera dentro del código, por otro lado, la 
clase “obstáculo” representaran aquellos autos enemigos del 
jugador. Para ambos casos el método será “dibujo”.  
El método es el encargado de dar las instrucciones a la 
clase para así realizar la acción. La función de este método 
“dibujo” es dibujar en pantalla el rectángulo que representara 
visualmente al jugador y así mismo a los obstáculos.La 
instrucción principal de este método será el comando a pygame 
para dibujar las formas de los autos. El método dibujo funciona 
a partir de un bucle.  
“Dibujo” usa pygame.drw.rect para si poder darle 
dimensiones al personaje y al obstáculo creando visualmente un 
rectángulo. La instrucción de este metodo es el siguiente 
permitiendo que en pygame tome forma  
Pygame.drw.rect(interfaz,color,self,forma)  
También utilizamos en método “mover” que dará las 
instrucciones a la clase para que se pueda cambiar de posición y 
para que el obstáculo tenga la simulación del movimiento hacia 
abajo. 

- Funciones y procedimientos: 
Estas funciones configuran la pantalla y dibuja los 
detalles del juego, organizan y reutilizan el código. Las 
funciones devolverán valor mientras que los procedimientos no. 
En este juego manejamos principalmente procedimientos ya que 
no se retornan valores.  
El procedimiento será el inicio del juego en el que ejecuta 
el flujo principal del juego y además gestiona los bucles.   
o Procedimiento 1: “Opción 1” Esta la encontramos en el 
principio del juego en el que utilizamos el Switch Case 
para iniciar el juego  
o Procedimiento 2: “Dibujo (Self, interfaz) Este 
procedimiento pertenece a las clases y dibuja los 
elementos en la pantalla  
o Función: mover (self,velocidad). Pertenece a la clase 
obstáculo y actualiza su posición para simular el 
movimiento

- Función para verificar las colisiones
  Para este utilizamos el bucle for y el condicional if. 

- Funciones para las opciones del menú de Tkinter
  def opcion_1(): 
mensaje["text"] = "Iniciando el juego"  # Muestra un 
mensaje  threading.Thread(target=iniciar_juego).start()

- Función principal del juego con pygame:
  def iniciar_juego(): 
screen = pygame.display.set_mode((600, 800))

## DIAGRAMA DE FLUJO DE DATOS  
<img width="446" height="412" alt="{47E7F728-B583-4824-929E-3F397A48B59E}" src="https://github.com/user-attachments/assets/21e2ea26-2f6d-44d9-b0bd-9bd74fb003c1" />


## 📎 Capturas (opcional)

<img width="675" height="354" alt="{207C58D4-9FEE-4609-B76E-02C0287E9528}" src="https://github.com/user-attachments/assets/d010bbb1-9728-47f9-bde4-1355750d8b9a" />
<img width="688" height="351" alt="{C4D72511-7696-4E0F-8006-1D42AC106F2B}" src="https://github.com/user-attachments/assets/99ebdfb8-4022-496f-be99-78df46ab1ec0" />
