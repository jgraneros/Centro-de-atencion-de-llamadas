
## Caso de uso: RegistrarLlamada

### Actor principal: Operador
### Precondiciones: El Operador se identifica y autentica
### Garantías de éxito: Se registra el llamado, se actualiza la disponibilidad de recursos

### Escenario principal de éxito

1. El siguiente caso de uso comienza cuando una Persona con síntomas se comunica con el centro de atención mediante un llamado telefónico.
2. El Operador atiende el llamado.
3. El Operador inicia un nuevo registro del llamado
4. El Operador solicita a la persona con sintomas sus datos personales [nombre, apellido, DNI, domicilio y telefono].
5. El Operador confirma el ingreso de los datos personales.
6. El sistema presenta la lista de selección de síntomas.
7. El Operador selecciona un síntoma de la lista.
8. El sistema presenta la lista actualizada con el síntoma seleccionado.
_Los pasos 7 - 8 se repiten hasta que se indique_
9. El Operador confirma los datos ingresados.
10. El sistema presenta el nivel de gravedad y el recurso asignado. 


