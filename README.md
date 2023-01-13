**"#NUMPY ACTIVITY"**

**0.- DATOS:**

He utilizado tres datasets obtenidos de:

\-<https://datos.gob.es/es/catalogo/ea0010587-balears-illes-por-municipios-y-fenomeno-demografico-mnpd-identificador-api-t20-e301-fenom-a2020-l0-23007-px>

\-<https://data.cityofnewyork.us/Housing-Development/Speculation-Watch-List/adax-9mit>

\-<https://ec.europa.eu/eurostat/databrowser/view/gov_10a_exp/defau>

Los he descargado en formato csv todos y los he cargado en jupyter notebook para poder trabajar con ellos.

En el proceso, he tenido que arreglarlos, seleccionando los datos de interés de mi análisis así como canviar el formato de los datos de string a float o íntegro para poder trabajar con ellos estadísticamente.

**1.-PRIMER DATASET**

El primero trata de datos de **las Islas Baleares**, donde nos indica el municipio así como también los nacidos vivos por residencia materna, los muertos fetales por residencia materna, los matrimonios por el lugar de residencia, los fallecidos por el lugar de residencia y el crecimiento vegetativo de cada municipio.

En este dataset solo he seleccionado los datos de interés. En mi caso, he seleccionado l*as muertes fetales por residencia materna.*

En media y en mediana, han muerto 165 fetos. Es más se observa como el máximo número de fetos muertos es 330 por residencia materna y como mínimo 0, el que indica que no siempre mueren.

Podemos ver como se producen muchas muertes fetales.

A continuación, vemos un boxplot de las muertes fetales que indica el rango de muertes desde el mínimo que es 0 al máximo que es 330 así como se marca en media (*línea naranja*) unos 165 muertos, lo que corrobora los datos obtenidos anteriormente. Y es más representativo.

![](images/muertesfetales.png)

**2.- SEGUNDO DATASET**

En el segundo dataset, encontramos **ventas de viviendas** con muchos indicadores.

Nosotros seleccionamos las valores de precios (*Price*) , ratio de capitalización (*cap_Rate*) i código postal (*Postcode*).

El mínimo precio de venta de las viviendas es y el máximo precio de venta es

Concluimos que hay un % de capitalización en media y un máximo de .

Es más, añadimos un diagrama de puntos para ver gráficamente el ratio de capitalización .

**3.- TERCERO DATASET**

Y el último dataset tiene datos del gobierno con años desdel 2012 al 2021 de diferentes países, incluyendo el gasto del gobierno de cada uno de ellos.

Primeramente seleccionamos un solo país. En este caso he seleccionado At que corresponde a Atenas desde 2012 -2021. Calculo la media de su gasto así como un diagrama de barras para ver su evolución.

A continuación, hay un gráfico lineal para ver más representativamente la evolución de At

Y por otro lado, selecciono todos las observaciones del año 2012, viendo el gasto de cada país en ese año.

Calculo el mínimo , el máximo y la media para ver que país destaca

**4.- CONCLUSIÓN:**

Obviamente la parte más complicada ha sido la de cargar los datos y arreglarlos para poder trabajar con ellos. Sin esa parte, las estadísticas no te salen.

Es más, no puedes ni visualizar los datos y entenderlos si no puedes cargarlos con la especificación correspondiente.

Todavía queda largo recorrido para aprender.
