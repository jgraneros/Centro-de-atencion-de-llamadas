# Porción #1

| *Escenario*  | *Pasos incluidos en el escenario del caso de uso* |
| :----------: | :-----------------------------------------------: |
| Flujo básico | 1 - 13                                            |

## Clases conceptuales identificadas mediante frases nominales

1. PersonaConSintomas
2. CentroDeAtencion
3. LlamadoTelefonico
4. Operador
5. RegistroDeLlamado
6. ~~DatosPersonales~~
7. ListaDeSeleccionDeSintomas
8. Sintoma
9. NivelDeGravedad
10. Recurso
11. AsignacionDeRecurso

## Asociaciones de alta prioridad

1. A es una parte lógica o física de B

        ~~DatosPersonales -- PersonaConSintomas~~
        Sintoma -- PersonaConSintomas

2. A está contenido lógica o físicamente en B

        Sintoma -- ListaDeSeleccionDeSintomas
        RegistroDeLlamado -- CentroDeAtencion
        Recurso -- CentroDeAtencion

3. A se registra en B

        LlamadoTelefonico -- RegistroDeLlamado
        Recurso -- PersonaConSintomas

## Asociaciones comunes
4. A es una descripción de B
5. A es una línea de una transacción o informe de B
6. A se conoce/registra/captura/informa/recoge en B
7. A es miembro de B

        Operador -- CentroDeAtencion

8. A es una subunidad organizativa de B
        Sintoma -- NivelDeGravedad
9.  A utiliza o gestiona B

        Operador -- RegistroDeLlamado
        Operador -- ListaDeSeleccionDeSintomas

10. A se comunica con B

        PersonaConSintomas -- CentroDeAtencion

11. A está relacionado con una transacción B

        PersonaConSintomas -- LlamadoTelefonico
        Operador -- LlamadoTelefonico

12. A es una transacción relacionada con otra transacción B
13. A está al lado de B
14. A es propiedad de B
15. A es un evento relacionado con B
        AsignacionDeRecurso -- Recurso
        AsignacionDeRecurso -- PersonaConSintomas

