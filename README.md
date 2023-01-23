**"#NUMPY ACTIVITY"**

**0.- DATOS:**

He utilizado tres datasets obtenidos de:

\-<https://datos.gob.es/es/catalogo/ea0010587-balears-illes-por-municipios-y-fenomeno-demografico-mnpd-identificador-api-t20-e301-fenom-a2020-l0-23007-px>

\-<https://data.cityofnewyork.us/Housing-Development/Speculation-Watch-List/adax-9mit>

\-<https://ec.europa.eu/eurostat/databrowser/view/gov_10a_exp/defau>

Los he descargado todos en formato *csv* y los he cargado en jupyter notebook para poder trabajar con ellos.

En el proceso, he tenido que arreglarlos, seleccionando los datos de interés de mi análisis así como canviar el formato de los datos de string a float para poder trabajar con ellos estadísticamente.

**1.-PRIMER DATASET**

El primer dataset son datos de **las Islas Baleares**, donde nos indica el municipio así como también los nacidos vivos por residencia materna, los muertos fetales por residencia materna, los matrimonios por el lugar de residencia, los fallecidos por el lugar de residencia y el crecimiento vegetativo de cada municipio.

En este dataset solo he seleccionado los datos de interés. En mi caso, he seleccionado l*as muertes fetales por residencia materna.*

En media y en mediana, han muerto 165 fetos. Es más se observa como el máximo número de fetos muertos es 330 por residencia materna y como mínimo 0, el que indica que no siempre mueren.

A continuación, añadimos un boxplot de las muertes fetales que indica el rango de muertes desde el mínimo que es 0 al máximo que es 330 así como se marca en media (*línea naranja*) unos 165 muertos, lo que corrobora los datos obtenidos anteriormente. Y es más representativo.

![](images/muertesfetales.png)

**2.- SEGUNDO DATASET**

En el segundo dataset, encontramos **ventas de viviendas** con muchos indicadores.

Nosotros seleccionamos las valores de precios (*Price*) , ratio de capitalización (*cap_Rate*) y código postal (*Postcode*).

El mínimo precio de venta de las viviendas es 500000y el máximo precio de venta es 90000000.

Concluimos que hay en media un 1488189.32 de capitalización y un máximo de 62000000.

Es más, añadimos un diagrama de puntos para ver gráficamente el ratio de capitalización por código postal.

![](images/capitalizaci%C3%B3n.png)

**3.- TERCERO DATASET**

Y el último dataset tiene datos del gobierno con años desdel 2012 al 2021 de diferentes países, incluyendo el gasto del gobierno de cada uno de ellos.

Primeramente, cargo solo la última columna correspondiente al gasto del gobierno e incluyo el mínimo ( 24.2), el máximo (62.8), la mediana (45.95) y la media (45.67) de toda la columna, lo que incluye todos los países y todo el periodo (2012-2021).

Y por otro lado, seleccionamos un solo país. En este caso he seleccionado At que corresponde a Austria desde 2012 -2021. Vuelvo a calcular el mínimo (48.6), el máximo (56.7), la mediana (51.15) y la media (51.58) de su gasto del gobierno.

Añado un histograma del gasto de gobierno de Austria.

**4.- CONCLUSIÓN:**

Obviamente la parte más complicada ha sido la carga de los datos y arreglarlos para poder trabajar con ellos. Sin esa parte, las estadísticas no te salen.

Es más, no puedes ni visualizar los datos y entenderlos si no puedes cargarlos con la especificación correspondiente.

Para esto, es importante tener en cuenta la naturaleza de los datos así como entender los errores que te salen o te pueden salir al cargarlos para así poder encontrar una solución.

Al mismo tiempo, veo como solo con numpy se puede hacer, sin necesidad de usar pandas.

No obstante, todavía queda largo recorrido para aprender.
