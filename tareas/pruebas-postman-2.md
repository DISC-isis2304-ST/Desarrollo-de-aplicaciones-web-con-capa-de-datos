# Pruebas con Postman - Parte 2

## Introducción
En esta tarea vamos a realizar pruebas para asegurarnos de que las consutlas avanzadas en nuestra aplicación de Parranderos funcionan correctamente. Utilizaremos Postman para enviar peticiones HTTP a los endpoints de nuestra aplicación y verificar las respuestas obtenidas. Esto nos permitirá validar que la lógica de negocio se ejecuta según lo esperado.

### Objetivos:
- Realizar pruebas de consultas avanzadas en la aplicación de Parranderos.
- Validar que los datos se procesan y almacenan correctamente en cada operación.
- Asegurarse de que los controladores manejan adecuadamente las solicitudes y respuestas.

## Preparación

Si no has seguido el tutorial desde cero, puedes descargar desde GitHub la parte anterior de la tarea estando en la carpeta de la aplicación con la siguiente instrucción:

```
  git clone -b ConsultasAvanzadas --single-branch https://github.com/DISC-isis2304-ST/Parranderos.git .
```
## Ayudas

El siguiente código HTML te permitirá visualizar los resultados de las pruebas en Postman

```
var template = `
<style type="text/css">
    .tftable {font-size:14px;color:#333333;width:100%;border-width: 1px;border-color: #87ceeb;border-collapse: collapse;}
    .tftable th {font-size:18px;background-color:#87ceeb;border-width: 1px;padding: 8px;border-style: solid;border-color: #87ceeb;text-align:left;}
    .tftable tr {background-color:#ffffff;}
    .tftable td {font-size:14px;border-width: 1px;padding: 8px;border-style: solid;border-color: #87ceeb;}
    .tftable tr:hover {background-color:#e0ffff;}
</style>
{% raw %}
Máximo grado de alcohol: {{response.mayorGrado}}<br>
Menor grado de alcohol: {{response.menorGrado}}<br>
Grado promedio de alcohol: {{response.promedioGrado}}<br>
 
<table class="tftable" border="1">
    <tr>
        <th>ID</th>
        <th>Nombre</th>
        <th>Grado Alcohol</th>
        <th>Tipo</th>
    </tr>
    
    {{#each response.bebidas}}
        <tr>
            <td>{{id}}</td>
            <td>{{nombre}}</td>
            <td>{{grado_alcohol}}</td>
            <td>{{tipo.nombre}}</td>
        </tr>
    {{/each}}
</table>
{% endraw %}
`;
 
function constructVisualizerPayload() {
    return {response: pm.response.json()}
}
 
pm.visualizer.set(template, constructVisualizerPayload());
```

## Actividad Sugerida

- Terminar de implementar las pruebas en Postman necesarias para probar el CRUD de la aplicación de Parranderos.
