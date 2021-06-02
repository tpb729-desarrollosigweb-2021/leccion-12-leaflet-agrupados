# Leaflet - mapas de puntos agrupados (*cluster maps*)
## Leaflet.markercluster
El complemento [Leaflet.markercluster](https://github.com/Leaflet/Leaflet.markercluster) simplifica la elaboración de mapas de puntos agrupados.

Para utilizarse, primero deben incluirse los enlaces a los archivos CSS y JavaScript del complemento. 

```html
<head>
  ...
  <link rel="stylesheet" href="https://unpkg.com/leaflet.markercluster@1.4.1/dist/MarkerCluster.css">
  <link rel="stylesheet" href="https://unpkg.com/leaflet.markercluster@1.4.1/dist/MarkerCluster.Default.css">
  <script src="https://unpkg.com/leaflet.markercluster@1.4.1/dist/leaflet.markercluster-src.js"></script>
</head>
```

Para generar el mapa de puntos agrupados, debe crearse un objeto de la clase ```L.markerClusterGroup``` y luego agregarle una capa de puntos individuales con la función ```addLayer()```.

```javascript
  var capa_puntos_agrupados = L.markerClusterGroup();
  capa_puntos_agrupados.addLayer(capa_puntos_individuales);
```

En el sitio de Leaflet.markercluster puede encontrar más información acerca de [como personalizar el mapa de puntos agrupados](https://github.com/Leaflet/Leaflet.markercluster#options).

Puede ver un ejemplo de un mapa de puntos agrupados en [https://tpb729-desarrollosigweb-2021.github.io/ejemplo-mapa-leaflet-agrupados/](https://tpb729-desarrollosigweb-2021.github.io/ejemplo-mapa-leaflet-agrupados/).

**Ejercicios**  
1. Utilice los mapas de sus tareas para generar una capa de puntos agrupados con íconos personalizados.
