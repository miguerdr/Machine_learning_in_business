# Machine_learning_in_business
## Introdución 
La compañía minera OilyGiant. Busca nuevos pozos en tres regiones, buscaremos la mejor region con menos riesgo y mayores beneficios para realizar estos nuevos pozos en las tres regiones demarcadas como 0, 1, 2

**Descripción de los datos**

Los datos de exploración geológica de las tres regiones se almacenan en archivos:

- id — identificador único de pozo de petróleo
- f0, f1, f2 — tres características de los puntos (su significado específico no es importante, pero las características en sí son significativas)
- product — volumen de reservas en el pozo de petróleo (miles de barriles).

## conclusiones

- No hay valores ausentes en ninguno de los tres DataFrame,
- Se eliminan la columna id ya que no aporta información importante
- Se entrena el modelo con regresión lineal en cada región
- La región 1, tiene el menor REMC, y el mejor Score
- Podemos observar que la diferencia del volumen para un pozo sin perdidas es muy superior a la de cualquier resultado de las 3 regiones
- Las mejores ganancias son para la región 1, ya que el volumen objetivo es menor
- El beneficio por la región 1 es mayor y el riesgo de perdida es del 1%
- El intervalo de confianza de la región 1, esta comprendido entre valores positivos
- La mayor parte de las regiones muestran una distribución normal, a excepción de la región 1 y 2, muestra una relación lineal positiva con con el target
	
Con el modelo de Machine learning, la empresa Oily Giant
	- Se recomienda perforar los pozos petroleros nuevos en la región 1, ya que es la que tiene menor riesgo, y valores mas altos en beneficio de acuerdo a la técnica de bootstrapping
