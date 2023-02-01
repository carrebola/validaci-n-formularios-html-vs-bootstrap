# Ejemplo de como validar formularios utilizando html5 o bootstrap

## HTML5
- Utilizamos recursos como 'required' en los inputs que queremos que tengan validación. 
- Podemos crear requerimentos como número máximo y mínimo de caracteres, valor máximo y mínimo en numeros, etc.
- El tipo de input también implicará requisitos, como por ejemplo en el caso de las emails
- También podemos usar patrones a partir de *expresiones regulares* con PATTERN

### Ventajas
    - Viene por defecto y no hay que programar
    - Podemos controlar el estado de los inputs mediante javascript utilizando su API de validación https://www.w3schools.com/js/js_validation_api.asp
    - Podemos aplicar estilos a los inputs según son validos o invalidas con la pseudoclase :valid :invalid

## BOOTSTRAP
- Usaremos igualmente las condiciones de html5
- El formulario debe tener la propiedad 'novalidated' para evitar la validación de html5
- Debemos detectar el evento submit para aplicar al formulario la clase 'was-validated' la cual mostrará el aspecto de los inputs según validen o no.
- ### Ventajas
- El aspecto por defecto es mejor y podemos modificarlo con sass
- Podemos crear divs con mensajes para inputs validos e invalidas con la clase valid-feedback y invalid-feedback
- Se ve igual en todos los navegadores