# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
_Taller 1 - BPMN_

## 👥 Integrantes del equipo
- Ana Lucia Quintero Vargas (anaquiva@unisabana.edu.co)
- Carlos Augusto Sánchez Lombana (carlossanlo@unisabana.edu.co)
- Diego Fernández Ramírez Tenjo (diegorate@unisabana.edu.co)
- Juan David Cetina Gómez (juancego@unisabana.edu.co)
- Mariana Salas Gutiérrez (marianasalgu@unisabana.edu.co)
- Mateo de Jesus Vanegas Correa (mateovaco@unisabana.edu.co)

## 🧠 Descripción general del trabajo
El presente taller tiene como objetivo modelar un proceso de negocio real, en este caso, de un hospital, utilizando la notación BPMN, identificando de forma clara los eventos, actividades, decisiones, actores y puntos críticos del flujo.

Para desarrollar esta actividad, la primera parte se realizó durante la clase, mientras que la otra en tiempo extracurricular. En la sesión de clase, utilizando marcadores y tablero, se definieron los actores, actividades y decisiones en el proceso de agendamiento de citas de La Clínica Salud Viva (caso base). Después, se modeló el proceso en la herramienta draw.io, escogida por permitir el trabajo colaborativo en tiempo real. Adicionalmente, para modelar correctamente los procesos, se investigó acerca de las buenas prácticas de BPMN. Posteriormente, se aplicó la misma metodología al proceso real del cliente asignado, correspondiente al proceso de entrega de resultados de laboratorio. Este, trata desde la realización del examen hasta la entrega de resultados al paciente y al médico
tratante, incluyendo retrasos por desconexión de sistemas. Finalmente, se documentó el trabajo en los informes correspondientes, describiendo el proceso, presentando y analizando el modelo final, y destacando las diferencias con el caso base.

## 🔧 Proceso de desarrollo

**Herramientas utilizadas y decisiones tomadas**

Originalmente, se planteaba utilizar la herramienta Astah para realizar los diagramas. Sin embargo, para la entrega final se decidió usar draw.io por su colaboración en tiempo real. 

La entrega se hace un repositorio de GitHub con la estructura solicitada. Tras finalizar el taller, cada integrante del grupo hizo un "fork" para tener su propia copia. Durante la clase, se utilizó un tablero y marcadores para los planteamientos iniciales. 

Para que la repartición del trabajo fuera equitativo, se definieron las tareas de cada integrante y una fecha estimada. Primero, se terminó la investigación acerca de las buenas prácticas de BPMN en el modelado de procesos de negocio para poder implementarlas en el modelo final. Después, se hizo el modelo. Con esto, finalmente, se documentó el proceso teniendo en cuenta las plantillas dadas en el repositorio: https://github.com/CesarAVegaF312/AREM-Taller_1_BPMN.git.

**¿Qué aspectos se modelaron primero? ¿Cómo se fue ajustando?**

Al inicio, se definieron los agentes del caso base. Después, se definieron los eventos (inicio, fin e intermedios). Posteriormente, las actividades principales y sus respectivos gateways. Luego, se añadió la interacción con bases de datos. Lo último que se hizo fue agregar actividades extras o complementarias a las principales para tener un flujo más detallado. Para el proceso de entrega de resultados de laboratorio se siguió el mismo flujo mencionado anteriormente. Conforme se avanzaba en los diagramas, se redefinieron los textos para mayor claridad y se organizaban los elementos con fines estéticos.

## 🧩 Análisis del modelo propuesto
- ¿Cómo se estructura el modelo entregado?

    **Caso base**

    - Agentes y entidades:
        1. Paciente.
        2. Sistema de citas médicas.
        3. Sistema de notificación.
        4. Base de datos.
        
    - Actividades principales: 
        1. Solicitar cita médica (Seleccionar especialidad, seleccionar médico, indicar fecha/hora).
        2. Verificar disponibilidad.
        3. Registrar cita.
        4. Enviar confirmación (correo/SMS).

    - Eventos:
        1. Inicio: en Paciente y Sistema de citas.
        2. Intermedios de mensaje: Solicitar agendamiento, Recibir notificación, Enviar confirmación.
        3. Fin: Tras confirmación o cierre por no reintentar.

    - Gateways:
        1. ¿Agenda disponible? (Exclusivo, ✕).
        2. ¿Notificación enviada con éxito? (Exclusivo, ✕).
        3. ¿Intentar con otras opciones? (Exclusivo, ✕).

    **Proceso de entrega de resultados de laboratorio**

    - Agentes y entidades:
        1. Paciente.
        2. Sistema de laboratorio.
        3. Personal de laboratorio.
        6. Médico tratante.
        5. Base de datos.
        
    - Actividades principales: 
        1. Solicitar cita de examen (Verificar agenda, agendar cita, notificar cita).
        2. Recolectar muestra (Recibir al paciente, etiquetar y registrar muestra).
        3. Procesar muestra.
        4. Subir resultados al sistema (Registrar resultados y validarlos).
        5. Habilitar acceso de resultados al paciente y enviar resultados al médico tratante.
        6. Notificar al paciente para que pueda consultar sus resultados.

    - Eventos:
        1. Inicio: en Paciente, Sistema de laboratorio, Personal de laboratorio y Médico tratante.
        2. Intermedios de mensaje: Recibe solicitud de cita, Notificar a paciente, Enviar resultados a médico, Recibir notificación. Retrasos.
        3. Fin: Paciente no desea reintentar o accede a los resultados, médico tratante tiene acceso a los resultados.

    - Gateways:
        1. ¿Agenda disponible? (Exclusivo, ✕).
        2. ¿Notificación enviada con éxito? (Exclusivo, ✕).
        3. ¿Sistema disponible? (Exclusivo, ✕).
        4. Compuerta paralela: Habilitar acceso al paciente y enviar resultados al médico.

- ¿Cómo representa las necesidades del cliente?

En el caso base, las necesidades del cliente son: agendar citas médicas y recibir notificaciones de estas. Entonces, las necesidades mencionadas anteriormente se ven representadas claramente en el diagrama, en el cual se incluye al paciente, el sistema de citas y el sistema de notificación. En este, se muestra el flujo de cómo el paciente pide una cita teniendo en cuenta la especialidad, el médico, la fecha y la hora, teniendo el escenario en el que se quiera realizar otro intento de agendamiento si el horario no llega a estar disponible. También, se muestra la interacción del sistema de citas con la base de datos para listar las opciones y guardar la información. Además, se tiene en cuenta el envío de mensajes por correo o SMS, incluyendo la posibilidad de que no se envíe con éxito y esta acción tenga que repetirse.

Por otra lado, en el caso del laboratorio, las necesidades del cliente son: recolectar la muestra, que esta se registre en el sistema del laboratorio, se valide y sea enviada al médico tratante y al paciente para que este pueda acceder a sus resultados. Por ello, estas necesidades se ven representadas en el diagrama mediante un flujo que inicia con la solicitud de cita de examen, la verificación de agenda y el envío de confirmación. Si no hay disponibilidad, el sistema notifica “Agenda no disponible” y permite reintentar. Después, el personal de laboratorio recibe al paciente, recolecta la muestra, la etiqueta y registra en el sistema. Luego, procesa la muestra y sube los resultados. Si el sistema no está disponible, se modela el retraso con un evento de temporizador y se reintenta la publicación tras el restablecimiento. Una vez registrados, los resultados pasan por validación y, mediante una compuerta paralela, se habilita el acceso al paciente y se envían al médico tratante de forma simultánea. Finalmente, se notifica al paciente que los resultados están disponibles y cada actor cierra su flujo al consultar la información correspondiente. Las interacciones con la base de datos quedan explícitas en los puntos de registro de muestras y registro de resultados, garantizando trazabilidad y consistencia de la información.

- ¿Qué supuestos se tomaron?

Para el caso base, se toman los siguientes supuestos:

1. La base de datos cuenta con información acerca de los médicos, sus especialidades y horarios disponibles.
2. El paciente puede cambiar especialidad/médico/fecha si no hay cupo.
3. El paciente proporciona datos de contacto válidos.
4. El flujo cubre creación de cita, no su modificación o cancelación.

Por otra parte, para el proceso de entrega de resultados de laboratorio se tienen los siguientes supuestos:

1. Existe una solicitud válida de examen.
2. La muestra se etiqueta con código de barras y se registra antes de procesarse.
3. Tras la validación, una compuerta paralela habilita acceso al paciente y envío al médico en forma simultánea.
4. El paciente accede a resultados por portal autenticado. El médico recibe notificación y puede consultar.
5. No se tienen en cuenta las repeticiones de exámenes de laboratorio por errores o resultados sospechosos.

## 📈 Diagrama final entregado
**Enlace al modelo final:** https://drive.google.com/file/d/1BJv5aFeUThF4R61ce-uZ2SmcK3yexryq/view?usp=sharing

## 📋 Tabla de actores, entidades o componentes (si aplica)

**Caso base**

| Nombre del elemento | Tipo | Descripción | Responsable |
|---------------------|------|-------------|-------------|
| Paciente        | Actor | Usuario que agenda una cita médica | Cliente |
| Sistema de citas        | Componente | Plataforma que gestiona las citas | Área de TI |
| Sistemas de notificación        | Componente | Envía confirmaciones y recordatorios al paciente por correo electrónico o SMS | Área de TI |
| Base de datos       | Entidad | Lleva el registro de las citas | Área de TI |

**Proceso de entrega de resultados de laboratorio**

| Nombre del elemento | Tipo | Descripción | Responsable |
|---------------------|------|-------------|-------------|
| Paciente        | Actor | Usuario que se realiza el examen y recibe los resultados | Cliente |
| Personal del laboratorio        | Actor | Encargado de procesar las muestras, validar resultados y registrarlos en el sistema | Clínica Salud Viva |
| Sistema de laboratorio        | Componente | Plataforma que almacena y gestiona los resultados de los exámenes | Área de TI |
| Médico tratante       | Actor | Profesional que interpreta los resultados y atiende al paciente | Clínica Salud Viva |
| Base de datos       | Entidad | Lleva el registro de los laboratorios | Área de TI |

## 🔍 Investigación complementaria
### Buenas prácticas BPMN en el modelado de procesos de negocio:
Al modelar procesos con BPMN, el objetivo principal es poder crear un lenguaje visual que cualquier persona pueda comprender. Esto requiere la adopción de buenas prácticas que son fundamentales para lograr un modelado efectivo y profesional.

### Resumen:
La investigación se centró en las buenas prácticas de BPMN, las cuales buscan convertir el modelado en una herramienta de comunicación efectiva. Se identificaron cuatro principios clave: la simplicidad, que sugiere evitar la complejidad excesiva en un solo diagrama; el uso correcto de la notación estandarizada, que diferencia con precisión los elementos del modelo; la coherencia visual, que ayuda a organizar el flujo para una lectura intuitiva; y la orientación hacia el lector, que exige que el modelo sea comprensible para cualquier persona sin conocimiento previo del proceso. Estas prácticas no son un conjunto rígido de reglas, sino directrices para que el modelo cumpla su propósito de comunicar de forma clara cómo funciona un proceso. La aplicación de estas prácticas es común en la industria, con ejemplos notables en el sector de la salud, donde se utilizan para mapear flujos críticos como la entrega de resultados de laboratorio. También son frecuentes en la banca y la logística, para coordinar procesos complejos que involucran a varios actores.

En el contexto del taller, se hizo un esfuerzo consciente por aplicar estas prácticas al modelar el proceso de entrega de resultados de laboratorio. Se priorizó la claridad, identificando a los actores en carriles separados para una asignación clara de responsabilidades. Además, se procuró el uso apropiado de la notación, empleando gateways para las decisiones lógicas y eventos intermedios de temporizador para representar las esperas en el proceso, como la del paciente antes de la cita o la del sistema ante una desconexión. La coherencia visual, que se logró con un flujo de izquierda a derecha, fue fundamental para que el diagrama fuera fácil de seguir. El proyecto, en su conjunto, demostró que estas buenas prácticas son cruciales para crear diagramas BPMN que realmente aportan valor, transformándolos en herramientas útiles para el análisis de procesos de negocio.

## 📚 Referencias
- [1] Dekhane, Anvita. *Dos and don'ts for process modeling*. 2025. https://www.uipath.com/community-blog/tutorials/dos-and-donts-for-process-modeling.
- [2] Trisotech. *BPMN Modeling Best Practices*. s. f. https://www.trisotech.com/bpmn-modeling-best-practices/.
- [3] Mathenge, Joseph. *Business Process Modeling Notation (BPMN): Getting Started with Visualization*. 2020. https://www.bmc.com/blogs/bpmn-business-process-modeling-notation.
- [4] Cardarello, Rafaela. *Buenas prácticas en BPMN*. s. f. https://qflowbpm.com/es/bpmn-mejores-practicas-2/.
- [5] BPMN Resources. *BPMN in Practice: Real-world examples and case studies*. s. f. https://bpmn.page/article/BPMN_in_practice_Realworld_examples_and_case_studies.html.

---

_Este documento hace parte de la entrega del taller BPMN del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._