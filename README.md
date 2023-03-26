# RedNeuronal_GA
Red Neuronal reajustando pesos usando Algotitmo Genético

Red neuronal básica, lee un archivo txt del siguiente formato:
"
40
18
4
95,48,83,178,72,10,162,42,20,159,176,379,184,70,6,16,187,197,3
"
-La primera linea indica cuantos valores serán ingresados (instancias)
-La segunda línea indica la cantidad de atributos
-La tercera línea indica la cantidad de clases en la red
-Las siguientes líneas están compuestas por la N cantidad de atributos separados con una coma, el último valor indica a cual de las k clases pertenece

Serán necesario ingresar los valores como cantidad de épocas, tasa de aprendizaje, momentum, cantidad de capas y cantidad de neuronas por capa

El algoritmo genético obtiene los valores iniciales de la red neuronal que son generados de manera aleatoria
El algoritmo muta el 10% del mejor resultado obtenido evaluando con la función fitness, mientras realiza una cruza del 50% entre el padre y madre para generar otros individos
Hay condiciones para evitar sobreajuste: si después de 4 iteraciones no se genera un mejor resultado se generan nuevos individos con valores aleatorios y se evalúa en la función fitness, así mismo, si se encuentran más de 5 valores iguales (en presición) respecto al mejor valor se muta en un tercio
Se estableció un máximo de 20 iteraciones

El archivo RedN.ipnyb es el resultado obtenido en google colab.
