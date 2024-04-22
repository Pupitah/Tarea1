# Sistema de Gestión de Pacientes en Hospital

## Descripción

Este sistema es una herramienta para gestionar la atención de pacientes en un hospital. Con él, los usuarios pueden registrar nuevos pacientes, asignar prioridades, ver la lista de espera y más. Su objetivo principal es mejorar la eficiencia en la atención médica, asegurando que los pacientes en situaciones críticas sean atendidos lo más rápido posible.

## Cómo compilar y ejecutar

Dado que el sistema está diseñado para ser accesible y fácil de probar, recomendamos usar [Repl.it](http://repl.it/) para una rápida configuración y ejecución. Sigue estos pasos para comenzar:

1. Visita [Repl.it](https://repl.it/).
2. Crea una nueva cuenta o inicia sesión si ya tienes una.
3. Una vez en tu dashboard, selecciona "New Repl" y elige "Import from GitHub".
4. Pega la URL del repositorio: `https://github.com/username/sistema-gestion-pacientes.git`.
5. [Repl.it](http://repl.it/) clonará el repositorio y preparará un entorno de ejecución.
6. Presiona el botón "Run" para compilar y ejecutar la aplicación.

## Funcionalidades

- Registro de pacientes con sus datos básicos y una prioridad inicial.
- Asignación o modificación de la prioridad de los pacientes.
- Visualización de la lista de espera de pacientes, ordenada por prioridad y hora de registro.
- Atención al siguiente paciente, respetando el orden de prioridad.

### Problemas conocidos:

- Debes colocar una edad con números sino falla el programa (en desarrollo).
- Quick fix a la hora de llegada de los pacientes usando aritmética. 


## Ejemplo de uso

**Paso 1: Registrar un Nuevo Paciente**

Se comienza registrando un nuevo paciente que acaba de llegar al hospital.

```
Opción seleccionada: 1) Registrar paciente
Ingrese el nombre del paciente: Ana Martínez
Ingrese la edad del paciente: 29
Ingrese el síntoma del paciente: Dolor abdominal agudo
```

El sistema registra a Ana Martínez con una prioridad inicial "Bajo" y guarda la hora actual de registro. La prioridad inicial puede ser ajustada más tarde basada en una evaluación médica más detallada.

**Paso 2: Asignar Prioridad a un Paciente**

Tras una evaluación inicial, el médico determina que el estado de Ana requiere atención prioritaria.

```
Opción seleccionada: 2) Asignar prioridad a paciente
Ingrese el nombre del paciente: Ana Martínez
Seleccione el nuevo nivel de prioridad (Alto, Medio, Bajo): Alto
```

El sistema actualiza la prioridad de Ana Martínez a "Alto", asegurando que será una de las próximas pacientes en ser atendida.

**Paso 3: Ver la Lista de Espera**

El usuario revisa la lista de espera para ver todos los pacientes y sus prioridades.

```
Opción seleccionada: 3) Mostrar lista de espera
```

La lista muestra a Ana Martínez en la parte superior, indicando su prioridad alta y que es la siguiente en línea para recibir atención.

**Paso 4: Atender al Siguiente Paciente**

Ana Martínez es llamada para ser atendida basándose en su prioridad.

```
Opción seleccionada: 4) Atender al siguiente paciente
```

El sistema muestra que Ana Martínez está siendo atendida y la elimina de la lista de espera.
