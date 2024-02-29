## Diagrama de casos de uso

![diagrama de casos de uso](out\use_case\use_case.png)


## Caso de uso: RegistrarLlamada

### Actor principal: Operador
### Precondiciones: El Operador se identifica y autentica
### Garantías de éxito: Se registra el llamado, se actualiza la disponibilidad de recursos

### Escenario principal de éxito

1. El siguiente caso de uso comienza cuando una Persona con síntomas se comunica con el centro de atención mediante un llamado telefónico.
2. El Operador atiende el llamado.
3. El Operador inicia un nuevo registro del llamado
4. El Operador solicita a la persona con sintomas sus datos personales [nombre, apellido, DNI, domicilio y telefono].
5. El sistema presenta el ingreso del nombre y apellido de la persona con sintomas.
6. El Operador ingresa el nombre y apellido de la persona con síntomas.
7. El sistema presenta el ingreso del domicilio y teléfono de la persona con síntomas
8. El Operador ingresa el domicilio y teléfono de la persona con síntomas.
9. El sistema habilita la confirmación de los datos personales ingresados.
10. El Operador confirma el ingreso de los datos personales.
11. El sistema presenta la lista de selección de síntomas.
12. El Operador selecciona un síntoma de la lista.
13. El sistema presenta la lista actualizada con el síntoma seleccionado.

_Los pasos 12 - 13 se repiten hasta que se indique_.

14. El Operador confirma los datos ingresados.
15. El sistema presenta el nivel de gravedad y el recurso asignado. 

### Extensiones

6a. El nombre ingresado no es válido.
    
    1. El sistema señala el error rechazando la entrada.

6b. El apellido ingresado no es válido.
    
    1. El sistema señala el error rechazando la entrada.

6c. Ambos, nombre y apellido ingresados no son válidos.
    
    1. El sistema señala el error rechazando la entrada.

8a. El domicilio ingresado no es válido.

    1. El sistema señala el error rechazando la entrada.

8b. El telefono ingresado no es válido.

    1. El sistema señala el error rechazando la entrada.

8c. Ambos datos,domicilio y telefono, ingresados no son válidos.

    1. El sistema señala el error rechazando la entrada.

12a. El síntoma que el Operador necesita seleccionar no se encuentra en la lista.

    1. El Operador ingresa la sugerencia del nuevo sintoma para su posterior aprobación y alta por parte del Administrador.

13a. El sistema determina que el nivel de gravedad es de NIVEL 1.

    1. EL sistema verifica la disponibilidad de turnos para el dia posterior a la llamada.
        1a. No hay turnos disponibles.
            1. El sistema presenta un mensaje indicando la situación.
    2. El sistema asigna el turno disponible al llamado.

13b. El sistema determina que el nivel de gravedad es de NIVEL 2.

    1. EL sistema verifica la disponibilidad de medicos para  la persona con sintomas.
        1a. No hay medicos disponibles.
            1. El sistema presenta un mensaje indicando la situación.
    2. El sistema asigna el medico disponible al llamado. 

13c. El sistema determina que el nivel de gravedad es de NIVEL 3.

    1. EL sistema verifica la disponibilidad de ambulancias para  la persona con sintomas.
        1a. No hay ambulancias disponibles.
            1. El sistema presenta un mensaje indicando la situación.
    2. El sistema asigna la ambulancia disponible al llamado. 