# FinalRN_Zazzali_Scardino

En este trabajo se busca poder clasificar a compuestos químicos de interés farmacéutico según su actividad tóxica o no tóxica. Para que un medicamento llegue finalmente al mercado se requieren más de 10 años y una gran inversión de dinero. La motivación se basa en lograr, mediante un modelo de redes neuronales, reducir tiempos y costos en las primeras etapas de la investigación de un nuevo medicamento.

Para esto se utilizó el dataset público de la competencia Tox 21 Data Challenge llevada a cabo en 2014. La misma buscó promover el uso de modelos de machine learning para la predicción de toxicidad de compuestos químicos. De los 12 efectos tóxicos evaluados por la competencia, se elige 1 para simplificar el trabajo. En este caso elegimos el efecto NR-ER que es una respuesta tóxica del receptor nuclear. Se eligió en base a su valor de activos/total de compuestos siendo éste un intermedio entre los valores de los 12 efectos.

tox21_DescriptorsCalc.ipynb permite calcular una serie de descriptores predefinidos que servirán como input para la red.

tox21_Model.ipynb realiza un acondicionamiento de los descriptores, una búsqueda de los hiperparámetros que obtienen los mejores resultados y un análisis de los resultados obtenidos.

nr-er.sdf es el dataset crudo para ese efecto tóxico otorgado por la competencia.

nr-er_removed.sdf es el dataset dado por la competencia y modificado para eliminar los compuestos agregados que no son de interés para la clasificación. 

nr-er_activity.txt contiene los valores target otorgados por la competencia.

Descriptores_test.csv contiene los descriptores ya calculados para el dataset de test.

nr-er_test_activity.txt son los targets del dataset de test para calcular los resultados finales. 
