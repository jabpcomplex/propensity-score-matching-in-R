# Propensity Score Matching (PSM)

El PSM pertenece a la clase de métodos estadísticos desarrollados para estimar los efectos del tratamiento no sesgados con datos no experimentales u observacionales para un resultado de interés (Rubin, 2006).

Esto se lleva a cabo de la siguiente forma: en una base de datos con información sobre el grupo de tratamiento y el grupo de control, tenemos datos sobre el resultado para el grupo de tratamiento, pero no hay información sobre los resultados fuera del tratamiento. De igual forma, para el grupo de control tenemos los resultados de control, pero no conocemos los resultados por unidad en tratamiento. Para inferir esta información (los efectos del tratamiento) hace falta parear los grupos de control y de
tratamiento. Este procedimiento solo se puede llevar a cabo si los grupos son pareados de tal forma que sean idénticos en el resto de características (covariables)
y que solo difieran por el tratamiento recibido. Si los grupos son comparables, entonces la diferencia media entre el resultado del grupo de tratamiento y el grupo de control representa el efecto causal promedio del tratamiento. Una forma de asegurar la comparabilidad entre los grupos y el pareamiento entre los casos es por medio de los puntajes de propensión o Propensity Scores (PS). En resumen, este método nos permite conocer información sobre dos contrafactuales: ¿cuál sería el resultado del grupo de tratamiento si este no hubiera recibido el tratamiento y cuál sería el resultado del grupo de control si este hubiera recibido el tratamiento? (Steiner y Cook, 2013).

En este sentido, el PSM es un método que permite encontrar efectos causales entre un tratamiento y un resultado esperado. Sin embargo, como gran parte del proceso depende de las covariables, es necesario que se cumpla el supuesto de **strong ignorability**.

Para que este supuesto se cumpla se tienen que cumplir los siguientes requerimientos: 

1) que las medidas de X estén correlacionadas con los resultados potenciales de los dos grupos;
2) si el proceso de selección y el modelo de resultados están basados en constructos latentes, estos tienen que estar especificados de manera correcta para dar cuenta del sesgo, y
3) los grupos de tratamiento y de control tienen que estar traslapados, es decir, contar con una zona común en los PS (Guo y Fraser, 2014).
