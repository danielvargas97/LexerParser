# Ejercicio Parser V1

Enunciado:
Teniendo como base un programa que posee un lexer y un parser que realiza operaciones matemáticas en notación infija. Este programa solo soporta sumas y multiplicaciones.
Se debe agregar soporte a restas y divisiones.

Solución:
Se modifica el lexer para agregar los tokens de resta y división que son *MINUS* y *DIVI*. Además, en el parser se agrega funciones para realizar resta y división.

Ejemplo:
Entrada:
((((1+1)*2)-9)/5)*10

Salida:
-10

Integrantes:
* Jhonathan Daniel Rojas Zora - 20151020041
* David Santiago Garces Benitez - 20151020032
* Daniel Alfonso Vargas Ortiz - 20152020009



Versiones posteriores pendientes:
- V2 Notación Posfija.
- V2.1 Archivo.


<pre>
G =< {E,T, F}, {+, ∗, num,(,)}, P, E >
E → E + T
E → T
T → T ∗ F
T → F
F → num
F → (E)
</pre>
