# **Análisis de Encuestas de indice mundial de la felicidad 2015 -2022**

![indice mundial de la felicidad!](./img/sonrie_bola_feliz.webp "indice mundial de la felicidad")

---

- [Importación de los Datos](#importación-de-los-datos)

  - [Nomenclatura de los datos](#nomenclatura-de-los-datos)

- [Limpiar y Filtrar los datos mas relevantes](#limpiar-y-filtrar-los-datos-mas-relevantes)

- [Estadisticas y Transformacion de los datos](#estadisticas-y-transformacion-de-los-datos)
- [Conclusión](#conclusión)

---

## **Importación de los Datos**

El Siguiente proyectos se basa de los datos del Índice global de felicidad de 2015 - 2022.

Los Datos lo encontrará [aquí](https://www.kaggle.com/datasets/mathurinache/world-happiness-report "indice mundial de la felicidad").

El índice mundial de la felicidad es una medida que se utiliza para evaluar el nivel de felicidad de los ciudadanos de diferentes países. Este índice se basa en una encuesta que se realiza cada año, en la que se pregunta a las personas sobre su percepción de la felicidad y bienestar en su vida.

El índice mundial de la felicidad se creó en 2012 por la ONU como una forma de medir el progreso de los países más allá del PIB. La idea detrás del índice de felicidad es que el bienestar de las personas no puede medirse únicamente en términos de su riqueza o ingresos, sino que es necesario tener en cuenta factores como la calidad de vida, la salud, la educación, la seguridad y la comunidad.

El índice mundial de la felicidad se elabora a través de una encuesta en la que se pregunta a las personas sobre su nivel de satisfacción con la vida, sus relaciones sociales, la libertad para tomar decisiones y la percepción de la corrupción en su país. Los resultados de la encuesta se utilizan para clasificar los países en función de su índice de felicidad, siendo los países con un índice más alto los considerados más felices.

Los resultados del índice mundial de la felicidad se utilizan para identificar las áreas en las que los países pueden mejorar para aumentar la felicidad de sus ciudadanos y para fomentar políticas públicas que promuevan el bienestar y la calidad de vida.

---

### **Nomenclatura de los datos**

La nomenclatura sobre el Índice global de felicidad se refiere a los términos y conceptos utilizados para describir y medir los Indices. Aquí te presento los términos usado en el datasets:

- **Country name:**

  País

- **Regional indicator:**

  Region donde pertenece el país

- **Ladder score:**

El "Ladder score" (puntuación en la escalera, en español) es una de las variables que se utiliza para medir el índice mundial de la felicidad. Se refiere a la evaluación subjetiva que una persona hace de su propia vida en una escala del 0 al 10, donde 0 es la peor vida posible y 10 es la mejor vida posible.

El "Ladder score" es una forma de medir la satisfacción con la vida de las personas y se utiliza como un indicador clave del bienestar subjetivo. Es decir, se basa en la percepción personal de las personas sobre su propia vida en lugar de en medidas objetivas como el ingreso per cápita o el nivel de educación.

La puntuación en la escalera se obtiene a través de una encuesta en la que se pregunta a las personas cómo evalúan su vida en general. Esta variable es una de las más importantes para la construcción del índice mundial de la felicidad, ya que refleja directamente la percepción de la felicidad y el bienestar subjetivo de las personas.

- **Standard error of ladder score:**

El "standard error of ladder score" (error estándar de la puntuación en la escalera, en español) es una medida estadística que se utiliza para indicar la precisión de la estimación del "Ladder score" en una muestra de la población.

El error estándar mide la variabilidad en los resultados de la encuesta y se calcula a partir de la desviación estándar de la muestra y el tamaño de la muestra. Cuanto mayor sea el tamaño de la muestra, menor será el error estándar y mayor será la precisión de la estimación del Ladder score.

En el contexto del índice mundial de la felicidad, el error estándar de la puntuación en la escalera indica cuánto puede variar la puntuación en la escalera en una muestra de la población en comparación con la puntuación real de la población completa. En otras palabras, el error estándar se utiliza para indicar el margen de error en la estimación del Ladder score de una muestra en particular.

El error estándar es importante porque puede ayudar a los investigadores a determinar si los resultados de la encuesta son significativos o no. Si el error estándar es muy alto, es posible que la muestra no sea representativa de la población completa y que los resultados de la encuesta no sean precisos. Por otro lado, si el error estándar es bajo, los resultados de la encuesta pueden ser considerados más precisos y representativos de la población completa.

- **upperwhisker:**

"Upper whisker" (bigote superior, en español) es una medida estadística que se utiliza para indicar la dispersión de los datos en un conjunto de valores.

En el contexto del índice mundial de la felicidad, el upper whisker se utiliza en los diagramas de caja y bigotes (boxplot, en inglés) para mostrar la distribución de los valores de Ladder score de los países en un año determinado. El boxplot representa la distribución de los valores de Ladder score mediante un rectángulo que se extiende desde el primer cuartil hasta el tercer cuartil, y una línea en el medio que representa la mediana.

El upper whisker se representa como una línea que se extiende desde el tercer cuartil hasta el valor máximo observado en los datos, y muestra la gama de valores más altos en los datos. En otras palabras, representa el límite superior de los valores de Ladder score observados en los países para un año determinado.

El upper whisker es importante porque permite identificar los valores extremos en la distribución de los datos. Si el upper whisker está muy alejado del resto de los valores, puede indicar que hay algunos países que tienen valores muy altos de Ladder score en comparación con el resto de los países. Por otro lado, si el upper whisker está cerca del tercer cuartil, puede indicar que la distribución de los valores de Ladder score es relativamente uniforme entre los países.

- **lowerwhisker:**

"Lower whisker" (bigote inferior, en español) es una medida estadística que se utiliza para indicar la dispersión de los datos en un conjunto de valores.

En el contexto del índice mundial de la felicidad, el lower whisker se utiliza en los diagramas de caja y bigotes (boxplot, en inglés) para mostrar la distribución de los valores de Ladder score de los países en un año determinado. El boxplot representa la distribución de los valores de Ladder score mediante un rectángulo que se extiende desde el primer cuartil hasta el tercer cuartil, y una línea en el medio que representa la mediana.

El lower whisker se representa como una línea que se extiende desde el primer cuartil hasta el valor mínimo observado en los datos, y muestra la gama de valores más bajos en los datos. En otras palabras, representa el límite inferior de los valores de Ladder score observados en los países para un año determinado.

El lower whisker es importante porque permite identificar los valores extremos en la distribución de los datos. Si el lower whisker está muy alejado del resto de los valores, puede indicar que hay algunos países que tienen valores muy bajos de Ladder score en comparación con el resto de los países. Por otro lado, si el lower whisker está cerca del primer cuartil, puede indicar que la distribución de los valores de Ladder score es relativamente uniforme entre los países.

- **Logged GDP per capita:**

"Logged GDP per capita" (PIB per cápita en escala logarítmica, en español) es una variable que se utiliza en el índice mundial de la felicidad para medir el ingreso económico de un país.

El PIB per cápita es una medida del valor total de la producción económica de un país dividido por su población. La escala logarítmica se utiliza para convertir esta variable en una forma más adecuada para su uso en el análisis estadístico, ya que el PIB per cápita puede variar enormemente entre los países y puede ser difícil de comparar en su forma original.

La escala logarítmica se utiliza porque la relación entre el PIB per cápita y la felicidad no es lineal. En otras palabras, un aumento de $1000 en el PIB per cápita puede tener un efecto más significativo en la felicidad de un país que un aumento de $1000 en un país más rico. Al tomar el logaritmo de los valores de PIB per cápita, los datos se transforman en una escala en la que los efectos de los aumentos en el ingreso se vuelven más uniformes.

La variable Logged GDP per capita es importante en el índice mundial de la felicidad porque el ingreso económico es uno de los factores que se cree que influyen en la felicidad de las personas. La variable Logged GDP per capita se utiliza para evaluar la relación entre el ingreso económico y la felicidad en diferentes países.

- **Social support:**

"Social support" (apoyo social, en español) es una variable que se utiliza en el índice mundial de la felicidad para medir el nivel de apoyo social percibido por las personas en un país.

Esta variable se refiere al grado en que las personas tienen una red de apoyo social, que puede incluir a amigos, familiares y otros miembros de la comunidad. El apoyo social puede tomar muchas formas, como el apoyo emocional, el asesoramiento práctico, la ayuda financiera y la participación en actividades sociales.

La variable de apoyo social en el índice mundial de la felicidad se mide mediante una encuesta en la que se pide a las personas que califiquen su nivel de acuerdo con afirmaciones como "¿Tiene alguien en quien confiar si tiene un problema?" y "¿Puede contar con alguien en caso de necesidad?".

El apoyo social es importante para la felicidad porque las personas que tienen una red de apoyo social percibida como fuerte pueden experimentar menos estrés y ansiedad y pueden tener una mayor sensación de bienestar emocional. Además, el apoyo social también puede ayudar a las personas a hacer frente a los desafíos de la vida, lo que puede mejorar su capacidad para experimentar emociones positivas y, en última instancia, su nivel de felicidad.

- **Healthy life expectancy:**

"Healthy life expectancy" (esperanza de vida saludable, en español) es una variable que se utiliza en el índice mundial de la felicidad para medir la salud percibida de la población en un país.

Esta variable se refiere al número de años que se espera que una persona viva en buen estado de salud, teniendo en cuenta los años que se espera que viva y la calidad de vida durante esos años. La salud percibida puede ser influenciada por una serie de factores, como la calidad de la atención médica, la nutrición, el acceso al agua potable y la seguridad alimentaria, entre otros.

La variable de esperanza de vida saludable en el índice mundial de la felicidad se mide mediante una encuesta en la que se pide a las personas que evalúen su propio estado de salud. También se utilizan datos de salud y esperanza de vida proporcionados por organismos internacionales como la Organización Mundial de la Salud (OMS) y la Organización para la Cooperación y el Desarrollo Económicos (OCDE).

La esperanza de vida saludable es importante para la felicidad porque la buena salud física y mental es un requisito previo para poder disfrutar de la vida en general. Las personas que disfrutan de una buena salud tienen más energía, son más capaces de realizar actividades y experimentan menos limitaciones y dolor físico. Todo esto puede contribuir a un mayor sentido de bienestar y felicidad en general.

- **Freedom to make life choices:**

"Freedom to make life choices" (libertad para tomar decisiones en la vida, en español) es una variable que se utiliza en el índice mundial de la felicidad para medir el grado de libertad percibida por las personas en un país para tomar decisiones importantes en su vida.

Esta variable se refiere a la percepción de las personas sobre su capacidad para tomar decisiones importantes en la vida, como decidir dónde vivir, elegir una carrera, formar una familia o tomar decisiones financieras. La libertad percibida puede verse afectada por muchos factores, como el nivel de democracia, la igualdad de género, el acceso a la educación y la seguridad personal.

La variable de libertad para tomar decisiones en la vida en el índice mundial de la felicidad se mide mediante una encuesta en la que se pide a las personas que evalúen su nivel de acuerdo con afirmaciones como "¿Tiene libertad para elegir la vida que desea?" y "¿Está satisfecho con su libertad para tomar decisiones importantes en su vida?".

La libertad para tomar decisiones en la vida es importante para la felicidad porque las personas que sienten que tienen la capacidad de tomar decisiones importantes en su vida pueden tener una mayor sensación de control y autonomía. Esto puede contribuir a una mayor satisfacción con la vida y a una mayor sensación de bienestar en general. Además, la libertad para tomar decisiones también puede estar asociada con un mayor sentido de responsabilidad personal y un mayor sentido de propósito en la vida.

- **Generosity:**

"Generosity" (generosidad, en español) es una variable que se utiliza en el índice mundial de la felicidad para medir la percepción de las personas sobre la generosidad y el altruismo en un país.

Esta variable se refiere a la percepción de las personas sobre la frecuencia con la que la gente en su país ayuda a los demás o dona a organizaciones benéficas. La generosidad percibida puede ser influenciada por una serie de factores, como las normas culturales, las prácticas religiosas, el nivel de desigualdad económica y la existencia de políticas sociales y de bienestar.

La variable de generosidad en el índice mundial de la felicidad se mide mediante una encuesta en la que se pide a las personas que evalúen su nivel de acuerdo con afirmaciones como "¿Ha donado dinero a una organización benéfica en el último mes?" y "¿Ha ayudado a un extraño en la última semana?".

La generosidad es importante para la felicidad porque las personas que perciben que hay un alto nivel de generosidad en su entorno pueden sentirse más conectadas con su comunidad y tener una mayor sensación de bienestar emocional. Además, la generosidad puede estar asociada con una mayor confianza en los demás y una mayor sensación de apoyo social, lo que puede contribuir a una mayor resiliencia y satisfacción con la vida.

- **Perceptions of corruption:**

"Perceptions of corruption" (percepciones de corrupción, en español) es una variable que se utiliza en el índice mundial de la felicidad para medir la percepción de las personas sobre la corrupción en un país.

Esta variable se refiere a la percepción de las personas sobre el nivel de corrupción en las instituciones públicas y en la sociedad en general. La corrupción puede manifestarse de diversas formas, como sobornos, tráfico de influencias, nepotismo y favoritismo, y puede ser perpetrada por personas en cargos políticos, funcionarios públicos y otros líderes de la sociedad.

La variable de percepciones de corrupción en el índice mundial de la felicidad se mide mediante una encuesta en la que se pide a las personas que evalúen su nivel de acuerdo con afirmaciones como "¿La corrupción es un problema importante en su país?" y "¿Confía en la policía y en el sistema judicial de su país?".

Las percepciones de corrupción son importantes para la felicidad porque la corrupción puede tener efectos negativos en la calidad de vida y el bienestar de las personas. La corrupción puede limitar el acceso a servicios públicos esenciales, como la atención médica y la educación, y puede erosionar la confianza en las instituciones públicas y en la democracia en general. Además, la corrupción puede estar asociada con un mayor nivel de desigualdad económica y una menor igualdad de oportunidades, lo que puede contribuir a una menor satisfacción con la vida y a una menor sensación de bienestar.

- **Ladder score in Dystopia:**

"Ladder score in Dystopia" (puntuación en la escala de la distopía, en español) es una variable que se utiliza en el índice mundial de la felicidad como una referencia para comparar la felicidad en diferentes países.

Esta variable representa la puntuación que se asignaría a un país que tendría las condiciones más adversas posibles, es decir, una distopía, donde las personas experimentarían la menor felicidad posible. Se utiliza como un punto de referencia para comparar la felicidad en otros países, ya que permite evaluar cómo las condiciones de vida en diferentes países se comparan con el peor escenario posible.

La variable "Ladder score in Dystopia" es un valor fijo que se utiliza en todos los cálculos del índice mundial de la felicidad. Su valor se basa en la puntuación más baja obtenida en la variable de "Ladder score" en la encuesta, y se utiliza para calcular la distancia relativa entre la puntuación de cada país y la puntuación de la distopía.

En resumen, "Ladder score in Dystopia" es una variable de referencia que se utiliza en el índice mundial de la felicidad para comparar la felicidad en diferentes países y evaluar cómo las condiciones de vida en cada país se comparan con el peor escenario posible.

- **Explained by: Log GDP per capita:**

"Explained by: Log GDP per capita" es una variable que se utiliza en el índice mundial de la felicidad para descomponer la puntuación total de felicidad de un país en diferentes factores que contribuyen a ella.

Esta variable representa la contribución de la variable "Log GDP per capita" (Producto Interno Bruto per cápita en logaritmo) a la puntuación total de felicidad del país. La idea detrás de esta variable es que, en general, los países con un mayor ingreso per cápita tienen una mejor calidad de vida y, por lo tanto, son más propensos a tener una mayor felicidad.

En la metodología del índice mundial de la felicidad, se utiliza un modelo estadístico que estima la contribución de diferentes variables a la felicidad de cada país. En este modelo, se incluyen variables como el ingreso per cápita, la esperanza de vida, el apoyo social, la libertad para tomar decisiones, la generosidad y la percepción de corrupción, entre otras.

"Explained by: Log GDP per capita" representa la contribución específica de la variable de ingreso per cápita a la felicidad total del país. Por lo tanto, cuanto mayor sea la puntuación en esta variable, mayor será la contribución de los ingresos a la felicidad del país.

- **Explained by: Social support:**

"Explained by: Social support" es una variable que se utiliza en el índice mundial de la felicidad para descomponer la puntuación total de felicidad de un país en diferentes factores que contribuyen a ella.

Esta variable representa la contribución de la variable "Social support" (apoyo social) a la puntuación total de felicidad del país. La idea detrás de esta variable es que las relaciones sociales y la calidad de los vínculos sociales son fundamentales para el bienestar y la felicidad de las personas.

En la metodología del índice mundial de la felicidad, se utiliza un modelo estadístico que estima la contribución de diferentes variables a la felicidad de cada país. En este modelo, se incluyen variables como el ingreso per cápita, la esperanza de vida, el apoyo social, la libertad para tomar decisiones, la generosidad y la percepción de corrupción, entre otras.

"Explained by: Social support" representa la contribución específica de la variable de apoyo social a la felicidad total del país. Por lo tanto, cuanto mayor sea la puntuación en esta variable, mayor será la contribución del apoyo social a la felicidad del país. En resumen, esta variable muestra cómo el apoyo social afecta la felicidad de las personas en un país determinado.

- **Explained by: Healthy life expectancy:**

"Explained by: Healthy life expectancy" es una variable que se utiliza en el índice mundial de la felicidad para descomponer la puntuación total de felicidad de un país en diferentes factores que contribuyen a ella.

Esta variable representa la contribución de la variable "Healthy life expectancy" (esperanza de vida saludable) a la puntuación total de felicidad del país. La idea detrás de esta variable es que la salud es un factor clave para el bienestar y la felicidad de las personas.

En la metodología del índice mundial de la felicidad, se utiliza un modelo estadístico que estima la contribución de diferentes variables a la felicidad de cada país. En este modelo, se incluyen variables como el ingreso per cápita, la esperanza de vida, el apoyo social, la libertad para tomar decisiones, la generosidad y la percepción de corrupción, entre otras.

"Explained by: Healthy life expectancy" representa la contribución específica de la variable de esperanza de vida saludable a la felicidad total del país. Por lo tanto, cuanto mayor sea la puntuación en esta variable, mayor será la contribución de la esperanza de vida saludable a la felicidad del país. En resumen, esta variable muestra cómo la salud afecta la felicidad de las personas en un país determinado.

- **Explained by: Freedom to make life choices:**

"Explained by: Freedom to make life choices" es una variable que se utiliza en el índice mundial de la felicidad para descomponer la puntuación total de felicidad de un país en diferentes factores que contribuyen a ella.

Esta variable representa la contribución de la variable "Freedom to make life choices" (libertad para tomar decisiones) a la puntuación total de felicidad del país. La idea detrás de esta variable es que la libertad para tomar decisiones es un factor clave para el bienestar y la felicidad de las personas.

En la metodología del índice mundial de la felicidad, se utiliza un modelo estadístico que estima la contribución de diferentes variables a la felicidad de cada país. En este modelo, se incluyen variables como el ingreso per cápita, la esperanza de vida, el apoyo social, la libertad para tomar decisiones, la generosidad y la percepción de corrupción, entre otras.

"Explained by: Freedom to make life choices" representa la contribución específica de la variable de libertad para tomar decisiones a la felicidad total del país. Por lo tanto, cuanto mayor sea la puntuación en esta variable, mayor será la contribución de la libertad para tomar decisiones a la felicidad del país. En resumen, esta variable muestra cómo la libertad afecta la felicidad de las personas en un país determinado.

- **Explained by: Generosity:**

"Explained by: Generosity" es una variable que se utiliza en el índice mundial de la felicidad para descomponer la puntuación total de felicidad de un país en diferentes factores que contribuyen a ella.

Esta variable representa la contribución de la variable "Generosity" (generosidad) a la puntuación total de felicidad del país. La idea detrás de esta variable es que la generosidad es un factor que puede influir en el bienestar y la felicidad de las personas.

En la metodología del índice mundial de la felicidad, se utiliza un modelo estadístico que estima la contribución de diferentes variables a la felicidad de cada país. En este modelo, se incluyen variables como el ingreso per cápita, la esperanza de vida, el apoyo social, la libertad para tomar decisiones, la generosidad y la percepción de corrupción, entre otras.

"Explained by: Generosity" representa la contribución específica de la variable de generosidad a la felicidad total del país. Por lo tanto, cuanto mayor sea la puntuación en esta variable, mayor será la contribución de la generosidad a la felicidad del país. En resumen, esta variable muestra cómo la generosidad afecta la felicidad de las personas en un país determinado.

- **Explained by: Perceptions of corruption:**

"Explained by: Perceptions of corruption" es una variable que se utiliza en el índice mundial de la felicidad para descomponer la puntuación total de felicidad de un país en diferentes factores que contribuyen a ella.

Esta variable representa la contribución de la variable "Perceptions of corruption" (percepción de corrupción) a la puntuación total de felicidad del país. La idea detrás de esta variable es que la corrupción puede afectar negativamente el bienestar y la felicidad de las personas.

En la metodología del índice mundial de la felicidad, se utiliza un modelo estadístico que estima la contribución de diferentes variables a la felicidad de cada país. En este modelo, se incluyen variables como el ingreso per cápita, la esperanza de vida, el apoyo social, la libertad para tomar decisiones, la generosidad y la percepción de corrupción, entre otras.

"Explained by: Perceptions of corruption" representa la contribución específica de la variable de percepción de corrupción a la felicidad total del país. Por lo tanto, cuanto mayor sea la puntuación en esta variable, mayor será la contribución de la percepción de corrupción a la falta de felicidad en el país. En resumen, esta variable muestra cómo la percepción de la corrupción afecta la felicidad de las personas en un país determinado.

- **Dystopia + residual:**

"Dystopia + residual" es una variable que se utiliza en el índice mundial de la felicidad para comparar la felicidad de un país con una situación imaginaria de "distopía" o infelicidad total.

La variable "Dystopia" es una puntuación fija que se utiliza para representar un estado hipotético de máxima infelicidad o distopía en el que se supone que todos los países tienen el peor rendimiento posible en todas las variables que se utilizan para medir la felicidad. La puntuación de "Dystopia" se mantiene constante en todas las ediciones del índice mundial de la felicidad, y su valor actual es de 1.972.

Por otro lado, la variable "Residual" es una variable estadística que se utiliza para representar la diferencia entre la felicidad real de un país y su felicidad esperada en función de su rendimiento en las diferentes variables que se utilizan en el modelo de felicidad. La variable residual puede tener valores positivos o negativos, lo que significa que algunos países pueden tener una felicidad mayor o menor que la que se espera en función de su rendimiento en las diferentes variables.

La variable "Dystopia + residual" se calcula sumando la puntuación de "Dystopia" y la variable "Residual", lo que representa una comparación de la felicidad real del país con una situación hipotética de máxima infelicidad y su diferencia con respecto a la felicidad esperada en función de su rendimiento en las diferentes variables.

En resumen, la variable "Dystopia + residual" se utiliza en el índice mundial de la felicidad para comparar la felicidad de un país con una situación hipotética de infelicidad total, y representa la diferencia entre la felicidad real del país y su felicidad esperada en función de su rendimiento en las diferentes variables que se utilizan para medir la felicidad.

[🔼](#análisis-de-encuestas-de-indice-mundial-de-la-felicidad-2015--2022)

---

## **Limpiar y Filtrar los datos mas relevantes**

- **Eliminar valores duplicados:**

Los datos duplicados pueden introducir errores en el análisis y deben eliminarse.

- **Revisar valores faltantes:**

Si hay valores faltantes, debe determinarse si es posible imputarlos o si deben eliminarse las filas correspondientes.

- **Verificar la consistencia de los datos:**

Los valores extremos o inesperados pueden ser señal de errores en la recolección de datos y deben verificarse y, si es necesario, corregirse.

- **Verificar la calidad de los datos:**

Los datos incompletos, inconsistentes o incorrectos pueden ser una señal de problemas en la calidad de los datos y deben ser corregidos.

- **Normalizar los datos:**

Los valores de los datos pueden estar en diferentes escalas o unidades, lo que puede dificultar la comparación entre ellos. Es posible que deba normalizar los datos para facilitar el análisis.

- **Verificar la precisión de los datos:**

los errores de entrada de datos pueden introducir errores en el análisis. Por lo tanto, debe verificar que los datos se ingresaron correctamente y hacer correcciones si es necesario.

- **Estandarizar los datos:**

Los nombres de columnas o variables pueden variar en diferentes conjuntos de datos. Para facilitar el análisis, es posible que deba estandarizar los nombres de las variables.

[🔼](#análisis-de-encuestas-de-indice-mundial-de-la-felicidad-2015--2022)

---

## **Estadisticas y Transformacion de los datos**

- **Gráfico de barras:**

Este tipo de gráfico es adecuado para mostrar la comparación de los resultados de diferentes países en el índice de felicidad. En este tipo de gráfico, cada país se representa con una barra vertical y la altura de la barra representa el índice de felicidad. Los países se pueden ordenar de mayor a menor índice de felicidad para hacer más fácil la comparación.

- **Gráfico de líneas:**

Este tipo de gráfico es útil para mostrar la tendencia del índice de felicidad a lo largo del tiempo. En este tipo de gráfico, se traza una línea que representa el índice de felicidad para cada año y se pueden comparar los cambios en el índice de felicidad a lo largo del tiempo.

- **Gráfico de dispersión:**

Este tipo de gráfico es adecuado para mostrar la relación entre dos variables, como el índice de felicidad y el PIB per cápita. En este tipo de gráfico, cada país se representa con un punto y la posición del punto en el gráfico muestra la relación entre las dos variables.

- **Mapa de calor:**

Este gráfico se puede utilizar para mostrar la distribución geográfica del índice de felicidad. Cada país se colorea según su valor de índice de felicidad, y los colores se pueden graduar para reflejar diferentes rangos de valores.

[🔼](#análisis-de-encuestas-de-indice-mundial-de-la-felicidad-2015--2022)

---

## **Conclusión**

- **Gráfico de barras:**

Esta gráfica muestra los 5 países con el mejor índice de felicidad para cada año en el conjunto de datos. Podemos observar que los países que aparecen en el top 5 varían de un año a otro, lo que indica que el índice de felicidad es un indicador cambiante y dinámico. También podemos ver que los países nórdicos (Dinamarca, Finlandia, Noruega, Suecia) tienen un alto índice de felicidad en muchos años, lo que sugiere que estos países han creado entornos propicios para la felicidad y el bienestar de sus ciudadanos. En general, esta gráfica nos da una idea de cómo ha evolucionado el índice de felicidad a lo largo del tiempo y qué países han estado en la cima en diferentes momentos.

- **Gráfico de líneas:**

Esta gráfica muestra la evolución del índice de felicidad en Perú a lo largo de los años. Podemos ver que el índice ha tenido altibajos a lo largo del tiempo, pero en general ha tendido a aumentar en la última década. Además, se ha agregado una línea horizontal y sombreado debajo de la línea que representa el promedio de felicidad en el periodo de tiempo considerado, lo que nos permite ver cómo el índice de felicidad de Perú ha fluctuado con respecto a este promedio. En general, esta gráfica nos permite ver de manera clara la tendencia del índice de felicidad en Perú y cómo este país se compara con el promedio de felicidad en el periodo de tiempo considerado.

- **Gráfico de dispersión:**

Esta gráfica muestra la relación entre el PIB per cápita y la puntuación de felicidad en cuatro países de América Latina: Perú, Chile, Argentina y Venezuela. Cada punto representa un país y su posición en el gráfico indica su PIB per cápita y su puntuación de felicidad. La línea de regresión muestra la tendencia general de la relación entre estas dos variables. En general, la gráfica sugiere una relación positiva entre el PIB per cápita y la puntuación de felicidad, aunque con algunas excepciones. Por ejemplo, Argentina tiene un PIB per cápita relativamente alto pero una puntuación de felicidad más baja que Perú, que tiene un PIB per cápita más bajo. Además, Venezuela se ubica en el extremo inferior de la gráfica, con un PIB per cápita bajo y una puntuación de felicidad muy baja. En resumen, esta gráfica nos ayuda a visualizar la relación entre dos variables importantes para entender la calidad de vida en distintos países.

- **Mapa de calor:**

Esta gráfica muestra el Índice Mundial de la Felicidad para el año 2022 en distintos países del mundo. Se utiliza un mapa de calor para representar los puntajes de felicidad, donde los países con colores más oscuros tienen puntajes más altos y los países con colores más claros tienen puntajes más bajos.

La escala de color utilizada en el mapa de calor va desde 0 hasta 10, y se utiliza una escala de colores verde-rojo (RdYlGn) para representar los distintos puntajes de felicidad. También se incluyen anotaciones y etiquetas para explicar la fuente de los datos utilizados y para personalizar la presentación del gráfico.

En general, esta gráfica permite visualizar de manera clara y fácilmente comprensible los países con puntajes de felicidad más altos y más bajos en todo el mundo en el año 2022.

[🔼](#análisis-de-encuestas-de-indice-mundial-de-la-felicidad-2015--2022)

---
