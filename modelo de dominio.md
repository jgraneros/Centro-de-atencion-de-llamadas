### Lista de categorias

Objetos tangibles o físicos

    RegistroDeLlamados
    Ambulancia
    ListadoDeSintomas
    RegistroDeRecursos
    RegistroDePoliticas

Especificaciones, diseños o descripciones de las cosas

Lugares

    CentroDeAtencion
    Domicilio
    CentroDeSalud

Transacciones

    Llamado

Lineas de transacción

    Recurso

Roles de la gente

    Operador
    PersonaConSintomas
    Medico
    Administrador

Contenedores de otras cosas

Cosas en un contenedor

Otros sistemas informáticos o electromecánicos externos al sistema

Conceptos abstractos

    Sintoma
    Turno
    DatosPersonales
    DNI
    NumeroTelefonico
    NivelDeGravedad
    NivelDelRecurso

Organizaciones

    CentroDeAtencion
    CentroDeSalud

Hechos

    Llamado

Procesos

Reglas y políticas

    PoliticaDeModificacionRelacionNivelRecurso
    PoliticaDeAsignacionDeTurnos
    PoliticaDeAsignacionDeRecursos
    PoliticaDeControlDeComunicacion
    PoliticaDeSeleccionDeSintomas
    PoliticaDeRegistroDeLlamada
    PoliticaDeDisponibilidadDeRecursos

Registros de finanzas, trabajo, contratos, cuestiones legales

Instrumentos y servicios financieros

Manuales, documentos, articulos de referencia, libros

### Asociaciones de prioridad alta

A es una parte lógica o física de B

    DNI -- DatosPersonales
    Domicilio -- DatosPersonales
    NumeroTelefonico -- DatosPersonales
    DatosPersonales -- PersonaConSintomas
    NumeroTelefonico -- CentroDeAtencion
    

A está contenido física o lógicamente en B

    RegistroDeLlamados -- CentroDeAtencion
    RegistroDeRecursos -- CentroDeAtencion
    RegistroDePoliticas -- CentroDeAtencion
    Sintoma -- PersonaConSintomas
    ListadoDeSintomas -- CentroDeAtencion
    Ambulancia -- Recurso
    Medico -- Recurso
    Turno -- Recurso

A es una descripción de B

    NivelDeRecurso -- Recurso   
    

A se registra en B

    Sintoma -- ListadoDeSintomas
    Llamado -- RegistroDeLlamados
    Recurso -- RegistroDeRecursos

    PoliticaDeModificacionRelacionNivelRecurso - RegistroDePoliticas
    PoliticaDeAsignacionDeTurnos -- RegistroDePoliticas
    PoliticaDeAsignacionDeRecursos -- RegistroDePoliticas
    PoliticaDeControlDeComunicacion -- RegistroDePoliticas
    PoliticaDeSeleccionDeSintomas -- RegistroDePoliticas
    PoliticaDeRegistroDeLlamada -- RegistroDePoliticas
    PoliticaDeDisponibilidadDeRecursos -- RegistroDePoliticas
    
    NivelDeGravedad -- Llamado
    Recurso - Llamado

A es miembro de B

    Operador -- CentroDeAtencion

A utiliza o gestiona B

    Operador -- RegistroDeLlamados
    Operador -- ListadoDeSintomas
    Operador -- RegistroDeRecursos

A se comunica con B

    PersonaConSintomas -- Operador
    Operador -- PersonaConSintomas

A está relacionado con una transacción B

    Operador -- Llamado
    PersonaConSintomas -- Llamado













