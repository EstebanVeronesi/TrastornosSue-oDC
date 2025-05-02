
This integrative project from the Data Science course in the Information Systems Engineering program applies the full CRISP-DM data mining process, aiming to improve population sleep quality through data analysis and predictive modeling.

**Conocimiento del negocio:**

*Objetivos del negocio:*

*Objetivo general:*

Los investigadores buscan reducir la incidencia de trastornos de sueño entre la población en un 20% dentro del próximo año.

*Objetivos específicos:*

  •	Identificar los principales factores asociados a una buena calidad del sueño.
  
  •	Identificar los factores asociados a la apnea del sueño y al insomnio.
  
  •	Identificar los factores asociados a una mala calidad del sueño.
  
  •	Proveer recomendaciones prácticas que sean fácil de entender y de aplicar para el público general.

*Criterios de éxito:*
  
  •	Cumplimiento del objetivo de reducir la incidencia de trastornos del sueño en un 20% (60 puntos).
  
  •	Cumplimiento de los plazos establecidos (20 puntos).
  
  •	Cumplimiento del presupuesto asignado (20 puntos).

*Entregables:*

  •	Informe estratégico con sugerencias y planes de acción basados en las relaciones encontradas entre los diferentes   trastornos o malos hábitos que afectan la calidad del sueño.
  
  •	Documento que detalla en desarrollo completo del proyecto utilizando la metodología CRIPS-DM.

*Restricciones:*

  •	Las recomendaciones deben ser comprensibles y utilizables por el público general, evitando el uso de terminología técnica y prefiriendo términos categóricos.
  
  •	Considerar aspectos éticos relacionados con la privacidad y la identidad de las personas.
  
  •	Asegurar que las recomendaciones sean inclusivas y aplicables a una amplia audiencia.

*Recursos disponibles:*

  •	Datos del estudio sobre la salud del sueño proporcionados por la catedra.

  •	Equipo de trabajo.

  •	Software de minería de datos.

  •	Apoyo de comitentes del proyecto.

*Objetivos de la minería de datos:*

  •	Desarrollar un modelo predictivo, con una precisión mínima del 90% y un recall mínimo del 80% en las clases necesarias, que ayude a encontrar patrones para evitar un sueño de mala calidad en personas que presenten trastornos del sueño.

  •	Encontrar al menos 10 premisas, que cuenten con al menos un 80% de confianza, que permitan encontrar patrones que se relacionan con un buen sueño mediante el uso de un algoritmo de asociación.

  •	Encontrar el peso que tiene cada atributo con la calidad del sueño utilizando SVM para complementar los diagnósticos, para esto necesitaremos un modelo con un nivel de precisión que este arriba de los 90%

Criterios de éxito:

  •	Elección correcta de los algoritmos. (50 pts)
  
  •	Lograr el cumplimiento de criterios de aceptación mínima en la eficiencia o precisión de los modelos. (30 pts)
  
  •	Interpretabilidad de los modelos para el cumplimiento de los objetivos. (20 pts)

*Restricciones:*

  •	Necesidad de mantener la confidencialidad y privacidad de los datos personales.

  •	Limitaciones en la disponibilidad de datos específicos o información detallada de los mismos.

  •	Balance entre la complejidad de los modelos y su interpretabilidad para el público general.


Conocimiento de los datos:

![image](https://github.com/user-attachments/assets/c51613ad-0358-4f65-9824-84907c555eac)

Con este grafico podemos ver la distribución de los cargos que ocupan las personas y a la vez nos permite identificar que hay muestras que contienen errores de ortografía, los cuales son:

•	Nurce.

•	Acountant.

•	Layer.

•	Murse.

Además, el puesto conocido como “Sales Representative” puede cambiarse por Salesperson.

![image](https://github.com/user-attachments/assets/dd1eb275-f620-43dd-bab5-540a06955623)

Con este grafico podemos observar que no hay errores de escritura aparentes en este atributo, vemos que el grupo más numeroso es el de las personas que no tienen ningún desorden del sueño.

![image](https://github.com/user-attachments/assets/c9cd6ea2-0068-455d-a578-533a2d816208)

En este grafico vemos que tenemos casi la misma cantidad de personas de ambos géneros lo cual lo vemos como una ventaja para el experimento, además, no se ven errores de ortografía en las muestras.

![image](https://github.com/user-attachments/assets/59dfa353-0967-4508-99fa-33453435d870)

Acá podemos observar que debería haber solo 3 categorías para este atributo las cuales debería ser y formadas por:

  •	NormalWeight: Normal, Normal Weiht, NormalWeight, Normal Weight.

  •	OverWeight: OverWeight, Overweight, Over weight.

  •	Obese.

![image](https://github.com/user-attachments/assets/0385e96b-138d-42aa-932d-5c060d2b40cc)

La forma en la que está planteado este atributo no es muy útil para la investigación y deberemos evaluar la forma en la que lo transformaremos.

![image](https://github.com/user-attachments/assets/67c73b70-6543-466d-bfcb-495ba36f52b9)

Con este histograma sobre el atributo Age podemos deducir que la edad de la población se encuentra dentro del rango 27 y 60 años y, además, no hay valores anómalos.

![image](https://github.com/user-attachments/assets/e69dab0e-5613-41c7-85ee-e08b5c86b042)

Los valores normales del atributo Daily Steps se encuentra dentro del rango 3.000 y 10.000.

El rango con mayor cantidad de muestras es 3.000 y 8.000. 

Se encuentran 2 valores anómalos que marcan que dos personas hicieron alrededor de 60.000 y 100.000 pasos en un día.

![image](https://github.com/user-attachments/assets/c7f0a47e-b7f0-45fe-ac59-353fcbdb427a)

Los valores normales de este atributo se encuentran en el rango 4-9.

Se encontró un valor anómalo, el cual es 81 siendo que debería estar en una escala de 4 a 9 según el rango presente.

![image](https://github.com/user-attachments/assets/76dd94ad-9b5c-45b6-bca8-22d9f38a31d6)

![image](https://github.com/user-attachments/assets/004aa6a1-b0c0-44f9-a35e-46501c3abf80)

![image](https://github.com/user-attachments/assets/a0cb7f28-92c8-4508-8f01-4cc2586c4ee2)

![image](https://github.com/user-attachments/assets/67c8b19a-d5cb-4d97-9dcb-385904faefda)

En estos 4 atributos (Heart Rate, Stress Level, Physical Activity Level y Sleep Duration) no se encontraron valores anómalos aparentes.

Lo único que podemos resaltar, dentro del atributo Stress Level, es que este puede ser tratado como un valor categórico.

**Preparación de datos:**

*Tratamiento de valores faltantes y errores:*

Utilizamos el operador “Filter Examples” con los siguientes filtros para eliminar valores nulos dentro de variables categóricas:

![image](https://github.com/user-attachments/assets/2d8bc5ba-6632-4e1a-8312-6a8070fdeea1)

Utilizamos el operador “Replace Missing Values” para reemplazar los valores nulos de los siguientes atributos numéricos por el promedio:

![image](https://github.com/user-attachments/assets/8e61d2d1-fa72-408e-a0fd-bc67267ec472)

Se realizaron los siguientes cambios, mediante el operador Map, en el atributo Occupation:

![image](https://github.com/user-attachments/assets/f3514dff-9d8c-430b-be17-a5980d8a731a)

Atributo Blood Pressure:

Como se indicó durante la fase de conocimientos de datos, ese atributo deberá ser modificado para que nos sea de utilidad por lo tanto se llevó a cabo el siguiente proceso, con las siguientes condiciones:

![image](https://github.com/user-attachments/assets/08a78712-0a2c-48a2-81c9-cd5835459940)


  1.	Se dividió el atributo Blood Pressure en 2 separándolo por el símbolo “/”, con esto surgieron dos nuevos atributos que serán llamados Systolic y Diastolic.

  2.	Se utilizo el operador Guess type para que se cambie el tipo de atributo al que necesitamos posteriormente.

  3.	Se genero un nuevo atributo llamado Blood Pressure a partir de la siguiente formula: if(Systolic > 120 || Diastolic > 80, "High", if(Systolic < 90 && Diastolic < 60, "Low", "Normal"))

  4.	Se eliminaron los atributos Systolic y Diastolic ya que no son necesarios.

Atributo Quality of sleep:

Este es el atributo que elegimos para predecir y centrar nuestro proyecto por lo que se decidió transformarlo de una escala numérica a una que contenga 3 categorías:

  •	Good: si la calidad del sueño es mayor a 7 puntos.

  •	Normal: si la calidad del sueño es menor o igual a 7 puntos y a su vez es mayor o igual que 6 puntos.

  •	Bad: si la calidad del sueño es menor a 6 puntos.

*Detección de anomalías:*

En este caso se realizó el método de observación mediante la información del análisis exploratorio de los datos en la fase de conocimiento de estos.

Se detectaron anomalías solo en el atributo Daily Steps la cual se solucionó mediante el método de clustering y posterior eliminación del clúster que incluía estos elementos.

*Selección de atributos:*

Se elimino el atributo “Sleep Duration” ya que tiene mucha relación con el atributo “Sleep Quality”.

**Modelado:**

*Modelo 1:*

![image](https://github.com/user-attachments/assets/1766df8e-6e73-4e9a-8fd6-43709fb10c64)


*Pasos:*
  1.	Utilizamos el operador Filter Examples para que solo nos queden las muestras cuyo valor en el atributo “Sleep Disorder” es diferente a None, para quedarnos con las personas que tienen desordenes del sueño.

  2.	Utilizamos el operador Select Attributes para eliminar los atributos “Age”, “Heart Rate” y “Occupation” ya que creemos que no son útiles para este modelo.

  3.	Utilizamos el operador Generate Attributes para crear un nuevo atributo “Pyshical Activity Level” categórico a partir de la misma columna que era numérica.

  4.	Utilizamos el operador Set Role para darle la etiqueta label al atributo “Sleep Quality”.

  5.	Utilizamos el operador Cross Validation, junto con el algoritmo Decision Trees, Apply Model y Performance.

*Modelo 2:*

![image](https://github.com/user-attachments/assets/f4d71999-17fd-4714-81ff-7d008bfd4d3a)

*Pasos:*

1.	Generamos nuevos atributos categóricos que serán necesarios en el próximo paso:

  a.	“Blood Pressure = High”: true cuando es High y false cuando no lo es (seria normal en este caso ya que son las dos opciones).

  b.	“Daily Steps = Ok:” true cuando la persona hizo más de 8000 pasos (valor recomendado para una buena salud), false cuando no.

  c.	“Stress Level”: low cuando es menor que 4, high cuando es mayor o igual que 7 y normal cuando es mayor o igual que 4, o menor que 7.

  d.	“Physical Activity Level”: low cuando es menor igual que 40, high cuando es mayor que 70 y normal mayor que 40, menor o igual que 70.

3.	Utilizamos el operador Select Attributes para eliminar los siguientes atributos (ya sea porque son valores numéricos y no nos son útiles, o porque fueron reemplazados por otro):

  a.	“Age”.
 
  b.	“Blood Pressure”.
 
  c.	“Daily steps”.
 
  d.	“Gender”.
 
  e.	“Heart Rate”.
 
  f.	“Occupation”.
  
4.	Utilizamos el operador Nominal to Binominal para transformar todos los atributos categóricos en atributos de true o false.

5.	Utilizamos el operador FP-Growth con un min requirement frequency para calcular los “elementos” que ocurren con frecuencia.

6.	Utilizamos el operador Create Association Rules para crear asociaciones a partir de los datos obtenidos con el operador FP-Growth.

*Modelo 3:*

![image](https://github.com/user-attachments/assets/e4cc6fdf-c24b-44da-ab81-24dc1a0a69d5)

*Pasos:*

  1.	Utilizamos el operador Nominal to Numerical con dummy coding en todos los atributos, menos “Sleep Quality”.

  2.	Utilizamos multiply para, a partir de este punto, generar los 3 modelos necesarios.

  3.	En los 3 casos se generará un atributo para cada posible salida del atributo “Sleep Quality” (Good, Normal, Bad) como nuevos atributos true/false.

  4.	Utilizamos el operador “Set Role” para asignarle la etiqueta label al atributo “Sleep Quality” que corresponde.

  5.	Utilizamos el operador Cross Validation para utilizar el algoritmo SVM y luego llevar a cabo una evaluación de performance.

**Validación:**

Para los modelos 1 y 3 decidimos utilizar como criterio “accuracy” por la facilidad que tiene para interpretar y medir resultados.

*Modelo 1:*

![image](https://github.com/user-attachments/assets/040a1e02-a320-4ca2-a85c-117942efd5e1)

Obtuvimos un modelo con un 94% de precisión y un recall balanceado y alto en las clases que necesitamos (para este caso decidimos ignorar la clase true bad ya que no la utilizaremos). 

Logramos superar los criterios definidos anteriormente de un 90% de precisión y el 80% de recall en las clases que nos son útiles.

*Modelo 2:*

![image](https://github.com/user-attachments/assets/ab76b93d-1977-4a10-a3da-d39378831af9)

Se encontraron 14 premisas con sus conclusiones que superan el 80% de confianza, superando los objetivos necesarios y marcando el buen rendimiento del algoritmo.

*Modelo 3:*

“Sleep Quality = Bad”

![image](https://github.com/user-attachments/assets/aa427b05-6d88-4b47-971f-4a6a5d23ecd9)

Sleep Quality = Good”

![image](https://github.com/user-attachments/assets/27127932-c3f4-4eeb-9cef-b2ae01763fae)

“Sleep Quality = Normal”

![image](https://github.com/user-attachments/assets/8094333d-814c-496b-b7b4-978021bb73d7)

En los 3 algoritmos logramos superar el 95% de precisión cumpliendo el objetivo de 90% que se decidió en los objetivos.

Además, casi todas las clases superan el 94% de recall y están balanceadas, a excepción de true true dentro del atributo “Sleep Quality = Bad”, la cual decidimos dejarla así por la poca cantidad de muestras y se estimo que no significara un problema para la conclusión.

**Implementación:**

*Resumen ejecutivo:*

*Key Findings:*

Good Sleep Quality: It was found that individuals with low stress levels and high levels of physical activity are more likely to achieve good sleep quality.

Normal Sleep Quality: Individuals with moderate stress levels and varying physical activity levels can achieve nearly desired sleep quality.

Influence of Body Weight and Physical Activity: Maintaining a normal weight and high physical activity (8000 steps daily) can significantly improve sleep quality, even in individuals with high stress levels.

Jobs at Risk for Sleep: People working as nurses or doctors tend to have more difficulties achieving quality sleep.

Sleep Quality: Sleep quality is influenced by a combination of factors, including stress level, body weight, and physical activity.

*We can define the following rules:*

  •	Low Stress Levels: Consistently associated with better sleep quality.

  •	High Physical Activity: Can improve sleep quality, especially in individuals who are overweight.

  •	Normal Weight: Maintaining a normal weight and adequate physical activity can counteract the negative effects of stress on sleep quality.

*Recommendations:*

Based on these findings, we can make the following recommendations:

  •	Implement stress management programs to improve sleep quality.

  •	Promote regular physical activity (3 to 5 days a week), especially for overweight individuals.

  •	Conduct continuous follow-ups to adjust recommendations according to changes in stress levels and physical activity.

  •	Pay special attention to individuals with jobs involving long waking hours or rotating shifts.







  
