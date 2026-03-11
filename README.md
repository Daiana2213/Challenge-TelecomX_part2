# Challenge-TelecomX_part1
-- Estado del proyecto: Finalizado.

  ## Introducción
El objetivo de este proyecto es el poder comprender la evasión de clientes en la empresa Telecom X. Por tanto para eso es necesario este analisis, dado que la evasion pasa cuando un cliente decide cancelar el servicio contratado con la empresa
Lo que a la larga representa una pardida directa de ingresos y puede afectar la estabilidad del negocio. Asi que el poder identificar los factores que influyen es vital para poder diseñar estrategias que permitan mejorar la retencio de clientes.

  ## Desarrollo
  ### Limpieza y Tratamiento de Datos
En esta parte del proyecto basicamente, se paso de tener datos "sucios" y desordenados a tener una tabla limpia y lista para analizar. En este caso al usar value_counts(), se descubrió que había 224 celdas con un espacio vacío (' ').
Por tanto esos espacion fueron convertidos en valores nulos reales (pd.NA) y luego se borraron esas filas con dropna(). Asegurando asi de trabajar solo con informacion completa. 
* Ademas que se aplanaron las columnas, pues eran datos que estaban guardados como en una lista dentro de una sola celda. Por eso se uso pd.json_normalize

### Analisis Exploratorio de Datos
Dentro de los hallazgos se identifico cuánta gente se estaba yendo. Siendo un grupo grande de mas de 7,000 clientes, la gran mayoría decide quedarse, pero hay un grupo considerable de casi 1,900 personas que cancelaron el servicio. 
Y esto nos da una señal de alerta para entender qué está pasando con ese porcentaje que abandona la empresa. Al revisar el tipo de contrato, vemos que los clientes que pagan mes a mes son los que más se van, probablemente porque no tienen un compromiso a largo plazo. 
* En cambio, quienes firman por uno o dos años suelen ser mucho más fieles y estables. Y tambien influye como pagan los clientes. Se descubrio que las personas que usan el cheque electrónico cancelan mucho más que aquellas que tienen sus pagos automatizados con tarjeta o transferencia. 

## Conclusión
Lo que se recomiendo con todo esto es el empezar a fomentar el compromiso a largo plazo. Ya sea que la empresa ofresca descuentos o beneficios exclusivos a quienes decidan cambiarse a planes de uno o dos años. De esta forma, el cliente siente que ahorra dinero y la empresa asegura su permanencia.
Siendo esto una forma en la que ambas partes ganen, siento otra cosas clave el poder facilitar el proceso de pago. Como el incentivar a los usuarios a registrar pagos automáticos en lugar de usar metodos manuales como el cheque electronico. 

* Esto no solo es más comodo para el cliente, sino que reduce las cancelaciones por olvido o por tener que tomar la decisión de pagar cada mes. Y para los clientes que prefieren mantener su flexibilidad mes a mes, se pueden crear programas de fidelización. Al ofrecerles mejoras en su servicio o premios por su antigüedad.  
