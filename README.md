# Uso de datos Lidar GEDI

![](img/GEDI_16_10-500x281.jpg)

Como parte de lo presentado en una entrada de mi blog https://carbajallosa.blogspot.com/2021/03/uso-de-datos-lidar-gedi-con-qgis.html,
en este repositorio se incluye archivos que fueron empleados y que les permite reproducir el procedimiento empleado.

## Capas empleadas

Se tomó en cuenta como área de interés la selva de Perú, dentro del Departamento de Ucayali, para dicha zona se descargó 
un modelo de elevación digital (DEM), sobre el cual se cargaron los datos del producto GEDI, en esta oportunidad se usaron
los que corresponden al [GEDI02_B](https://lpdaac.usgs.gov/products/gedi02_bv001/).

En específico se trabajó con el siguiente archivo que puede ser descargado:

https://e4ftl01.cr.usgs.gov/GEDI/GEDI02_B.001/2020.07.17/GEDI02_B_2020199213433_O09046_T02722_02_001_01.h5



Cita:

Dubayah, R., Tang, H., Armston, J., Luthcke, S., Hofton, M., Blair, J. (2020). <i>GEDI L2B Canopy Cover and Vertical Profile Metrics Data Global Footprint Level V001</i> [Data set]. NASA EOSDIS Land Processes DAAC. Accessed 2021-03-22 from https://doi.org/10.5067/GEDI/GEDI02_B.001 <span><a href="javascript:"><img class="citavipicker" identifier="10.5067/GEDI/GEDI02_B.001" identifiertype="1" src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz48IURPQ1RZUEUgc3ZnIFBVQkxJQyAiLS8vVzNDLy9EVEQgU1ZHIDEuMS8vRU4iICJodHRwOi8vd3d3LnczLm9yZy9HcmFwaGljcy9TVkcvMS4xL0RURC9zdmcxMS5kdGQiPjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0iRWJlbmVfMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiIHdpZHRoPSIxNnB4IiBoZWlnaHQ9IjE2cHgiIHZpZXdCb3g9IjAgMCAxNiAxNiIgZW5hYmxlLWJhY2tncm91bmQ9Im5ldyAwIDAgMTYgMTYiIHhtbDpzcGFjZT0icHJlc2VydmUiPjxnPjxnPjxwYXRoIGZpbGw9IiNGRkZGRkYiIGQ9Ik04LjAwMSwxNS41QzMuODY0LDE1LjUsMC41LDEyLjEzNiwwLjUsOGMwLTQuMTM1LDMuMzY1LTcuNSw3LjUwMS03LjVTMTUuNSwzLjg2NCwxNS41LDhTMTIuMTM3LDE1LjUsOC4wMDEsMTUuNXoiLz48cGF0aCBmaWxsPSIjRDUyQjFFIiBkPSJNOC4wMDEsMUMxMS44NiwxLDE1LDQuMTQxLDE1LDhzLTMuMTM5LDctNi45OTksN0M0LjE0LDE1LDEsMTEuODU5LDEsOFM0LjE0LDEsOC4wMDEsMSBNOC4wMDEsMEMzLjU4MiwwLDAsMy41ODIsMCw4czMuNTgyLDgsOC4wMDEsOEMxMi40MTgsMTYsMTYsMTIuNDE4LDE2LDhTMTIuNDE4LDAsOC4wMDEsMEw4LjAwMSwweiIvPjwvZz48cGF0aCBmaWxsPSIjRDUyQjFFIiBkPSJNNi43NDUsMTIuNTg5Yy0wLjIyNywwLjEyMi0wLjQ5NywwLjI0Ny0wLjY4NCwwLjI0N2MtMC4zMTgsMC0wLjUwMS0wLjE2NC0wLjUwMS0wLjQ1MmMwLTAuMjA3LDAuMTQtMC4zNzUsMC41OTUtMC42MjJjMS41NDktMC45MDQsMi41OTQtMi4yNzIsMi41OTQtMy43MjFjMC0wLjgyNS0wLjIyNy0xLjExOS0wLjY4MS0xLjExOWMtMC4xMzUsMC0wLjMyLDAuMjE5LTAuNjM2LDAuMjE5SDcuMTU3QzYuMTAyLDcuMTQzLDUuMzMzLDYuMjY0LDUuMzMzLDUuMjNjMC0xLjE1MiwwLjk1OC0yLjAwNiwyLjI4LTIuMDA2YzEuNzc3LDAsMy4wNTMsMS4zNzMsMy4wNTMsMy40M0MxMC42NjYsOS4yMTUsOS4yMDMsMTEuMjcsNi43NDUsMTIuNTg5Ii8+PC9nPjwvc3ZnPg" style="border: 0px none!important;width: 16px!important;height: 16px!important;margin-left:1px !important;margin-right:1px !important;" title="Añadir títulos al proyecto de Citavi utilizando el DOI" existsinproject="0"></a></span>

![](img/zona_estudio.png)

También se uso un plugin de QGIS denominado [Qgis2threejs](https://github.com/minorua/Qgis2threejs) para generar una vista 3D con los datos de GEDI luego de 
ser convertidos al formato geojson, para ello se usó un scrip de Python denominado [GEDI-subsetter](https://git.earthdata.nasa.gov/projects/LPDUR/repos/gedi-subsetter/browse).

![](img/vista_qgis2threejs.png)


