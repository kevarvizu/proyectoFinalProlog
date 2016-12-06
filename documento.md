#INTRODUCCIÓN
##que es la pogramación lógica?
La Programación Lógica estudia el uso de la lógica para el planteamiento de problemas y el control sobre las reglas de inferencia para alcanzar la solución automática.

La Programación Lógica, junto con la funcional, forma parte de lo que se conoce como Programación Declarativa, es decir la programación consiste en indicar como resolver un problema mediante sentencias, en la Programación Lógica, se trabaja en una forma descriptiva, estableciendo relaciones entre entidades, indicando no como, sino que hacer, entonces se dice que la idea esencial de la Programación Lógica es:

__Programa= lógica + control__

Lógica (programador): hechos y reglas para representar conocimiento

Control (interprete): deducción lógica para dar respuestas (soluciones)

La programación lógica intenta resolver lo siguiente:

Dado un problema S, saber si la afirmación A es solución o no del problema o en que casos lo es. Además queremos que los métodos sean implantados en maquinas de forma que la resolución del problema se haga de forma automática

La programación lógica: construye base de conocimientos mediante reglas y hechos

Regla: implicación o inferencia lógica que deduce nuevo conocimiento, la regla permite definir nuevas relaciones apartir de otras ya existentes

##campos de aplicación

* Sistemas Expertos , donde un Sistema de información mita las recomendaciones de un experto sobre algún dominio de conocimiento.

* Demostración automática de teoremas, donde un programa genera nuevos teoremas sobre una teoría existente.

* Reconocimiento de lenguaje natural, donde un programa es capaz de comprender (con limitaciones) la información contenida en una expresión lingüística humana.

* Inteligencia artificial

* Sistemas de información

#problematica
El problema considerado para este proyecto es una situacion sumamente cotidiana en la que si no todos, la mayoria de los usuarios la comparten. Esto es sufrir una falla automotriz. Una persona promedio con automovil sufre varias fallas mecanicas al año, con lo cual se dio a la tarea de emplear un software que de un diagnostico previo hacia su posible falla. 

#justificación

La utilización de este sistema proveerá de un diagnóstico del automóvil, con el cual podremos tener una vista previa hacia una solución a la falla. Evitándonos cometer algún error humano o el ahorro de un chequeo para después corregir la falla. Se obtendrá una inclinación más rápida hacia el por qué el automóvil está fallando.

#desarrollo
A continuación, se presentan las reglas que el sistema sigue para arrojar un diagnostico. cada banco de preguntas tienes una inclinación hacia un tipo de problema automotriz (**aceite, suspención, electrico, etc**) el cual tiene preguntas especificas, contestadas que si, arroja un diagnostico hacia el tipo de problema que tenga el auto.

__aceite__:- cambio_aceite,
	pregunta('tienes problemas de motor?'),
	pregunta('su automovil gasta mas combustible de lo debido?'),
	pregunta('su motor se escucha muy ruidoso? '),
	pregunta('tiene problemas para arrancar el veiculo en frio?'),
	pregunta('siente que su motor tiene menos fuerza que antes? ').


__suspension__:- alineacion_direccion,
	pregunta('tienes problemas de la suspencion?'),
	pregunta('tiene su volante neutral y el auto gira?'),
	pregunta('ha notado que alguna llanta se desgasta mas? '),
	pregunta('su volante se mueve bastante y tiembla?').

__electronico__:- bateria_agotada,
	pregunta('tienes problemas electricos?'),
	pregunta('sus faros titilan o encienden con poca fuerza?'),
	pregunta('el estereo no enciende?'),
	pregunta('el auto emite un crack cuando lo enciende?'),
	pregunta('el auto no enciende de ninguna manera?'),
	pregunta('su bateria es muy vieja?').

__frenos__:- cambio_frenos,
	pregunta('tienes problemas con tus frenos?'),
	pregunta('cuando frenas escuchas un chillido agudo?'),
	pregunta('al frenar siente que tarda mas? ').

__computadora__:- check_egine,
	pregunta('la luz check egine se encendio en tu tablero?'),
	pregunta('la luz se mantiene encendida todo el tiempo?').

__sonido__:- cambio_bocina,
	pregunta('tienes problemas con alguna bocina?'),
	pregunta('la bocina no se escucha nada?'),
	pregunta('tu auto tiene suficiente bateria?').

#resultados

