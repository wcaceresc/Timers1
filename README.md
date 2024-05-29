# Timers1
Codigo que levanta 3 Timers y hace papadear x3 leds a diferentes razones de tiempo


El siguiente proyecto consiste en un codigo creado para encender 3 leds a diferentes razones de tiempo
Led 1 a 25ms
Led 2 a 500ms
Les 3 a 1s
El codigo consta de 3 fases, en la primera parte seteamos como salidas PA5, PA6 Y PA7 Como salidas 
![Captura de Pantalla 2024-05-29 a la(s) 06 21 04](https://github.com/wcaceresc/Timers1/assets/161264041/64547b3c-1dee-4524-8c59-e625fde7bcba)
En la segunda fase configuramos los timers en este caso use TIM22, TIM21 y Tim2 para los led respectivos, tambien se 
nos da la condicion de que hay que calcular el valor de ARR asumiendo que utiliza el HSI de 16Mhz y Prescaler de 1600
para lo cual utilizamos las formulas y calculamos, primero la frecuencia del temporizador timer=160000000/15999+1 
timer=1000 luego calculamos el ARR para el parpadeo de 1s. 500ms y 250ms. ejemplo ARR= (1 * 16000000)/16000 -1 
Arr= 999 y asi sucesivamente con los demas. y nos quedan de esta forma: ARR´s  999, 499 y 249  como podemos observar
en esta imagen

![Captura de Pantalla 2024-05-29 a la(s) 06 21 36](https://github.com/wcaceresc/Timers1/assets/161264041/ef48755d-cd60-40d6-8ebe-7c804a19e36d)


y por ultimo agegamos el ciclo para que este constantemente repadsando los valores y logre encender los distintos leds
![Captura de Pantalla 2024-05-29 a la(s) 06 22 04](https://github.com/wcaceresc/Timers1/assets/161264041/55878b17-b6e4-438f-a660-ab6f0562c6fe)



aqui adjunto el link del video demostrativo de su funcionamiento.

