## Cómo Compilar y Ejecutar
Dado que el sistema está diseñado para ser accesible y fácil de probar, recomendamos utilizar Repl.it para una configuración y ejecución rápidas. Sigue estos pasos para empezar:

- Visita Repl.it.
- Crea una cuenta nueva o inicia sesión si ya tienes una.
- Una vez en tu panel de control, selecciona "Nuevo Repl" y elige "Importar desde GitHub".
- Pega la URL del repositorio: https://github.com/Pupitah/Tarea1/edit/main/README.md
- Repl.it clonará el repositorio y preparará un entorno de ejecución.
- Presiona el botón "Run" para compilar y ejecutar la aplicación.
- METODO ALTERNATIVO: Ingresar directamente al LINK: https://replit.com/@lucas123kario/Tarea-1

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
