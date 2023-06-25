
# DATOS DE ENTRADA
Los datos de entrada son todos los puntos de la nube de puntos etiquetados como una hoja.


![Creacion de Mascara](https://github.com/Brayanjurado1325/Longitud-de-hojas/blob/main/Imagenes/1.png)

Inicialmente se recibe el vector con los puntos etiquetados como hoja, si el tamaño de este vector es mayor a los 1024 es necesario reducir este valor, para esto se realiza un muestreo para que la nube de puntos tenga un menor tamaño. 

![Creacion de Mascara](https://github.com/Brayanjurado1325/Longitud-de-hojas/blob/main/Imagenes/2.png)


# CREACION DE GRAFOS

![Creacion de Mascara](https://github.com/Brayanjurado1325/Longitud-de-hojas/blob/main/Imagenes/3.png)


## Crear formato para aplicar metodo Dijkstra.
Para poder aplicar el método Dijkstra es necesario hacer crear un Dataframe teniendo como base los datos del grafo que se ha creado a partir de la nube de puntos tipo hoja, este Dataframe debe tener la estructura que se muestra a continuacion, donde se agrupan todas las conexiones del grafo y también se calcula su distancia euclídea entre los dos puntos, los valores de origen y destino hacen referencia al índice dentro del vector donde se encuentran estos puntos. 

![Creacion de Mascara](https://github.com/Brayanjurado1325/Longitud-de-hojas/blob/main/Imagenes/4.png)

## Aplicacion de Metodo de Dijkstra.

Una vez aplicado el algoritmo que tiene como entrada los puntos de origen y destino, el algoritmo nos devuelve los saltos que debe seguir la ruta mínima con el menor costo, finalmente para encontrar la distancia se realiza la suma de las distancia entre los saltos. 
