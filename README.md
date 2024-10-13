## StateChart de un Sensor-Sistema-Actuador

El LED puede estar en diferentes modo, cambiando de estado según los eventos recibidos y ajustando el temporizador y el estado del LED en consecuencia para implementar los efectos visuales necesarios.

### EVENTOS

- EV_LED_01_TURN_ON / TURN_OFF: Enciende o apaga el LED.
- EV_LED_01_BLINKING_ON / BLINKING_OFF: Activa o desactiva el parpadeo del LED.
- EV_LED_01_PULSE_ON / PULSE_OFF: Inicia o detiene un pulso.
- EV_LED_01_PULSE_DCYCLE_ON / DCYCLE_OFF: Activa o desactiva el ciclo de pulso.
- EV_LED_01_TWO_PULSES_ON / OFF: Activa o desactiva dos pulsos.

### ACCIONES

- led = 1 / 0: Activa o desactiva el LED.
- timer = MAX_PERIOD_xxx: Establece el temporizador al periodo máximo para diferentes modos.
- pulse = 1 / 2 : Ajusta el número de pulsos en el estado correspondiente.
- timer--: Disminuye el valor del temporizador en cada transición.
