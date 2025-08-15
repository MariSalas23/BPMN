# 🗒️ Registro de Trabajo en Clase - Taller 1

## 📆 Fecha de la sesión

9 de agosto de 2025

## 👥 Integrantes presentes
- Ana Lucia Quintero Vargas (anaquiva@unisabana.edu.co)
- Juan David Cetina Gómez (juancego@unisabana.edu.co)
- Carlos Augusto Sánchez Lombana (carlossanlo@unisabana.edu.co)
- Mateo de Jesus Vanegas Correa (mateovaco@unisabana.edu.co)
- Diego Fernández Ramírez Tenjo (diegorate@unisabana.edu.co)
- Mariana Salas Gutiérrez (marianasalgu@unisabana.edu.co)

## 🧠 Actividades realizadas en clase

- ¿Qué se discutió con el equipo?

Durante la sesión se discutió con el equipo todos los pormenores relacionados con la realización del taller, específicamente el proceso de agendamiento de citas del caso. En primer lugar, se establecieron las herramientas que se emplearían para facilitar el trabajo en equipo y la diagramación del problema. Posteriormente se establecieron los actores, el flujo de las actividades y las interacciones principales en el proceso. Se definieron tres actores principales: el paciente, el sistema de citas y el sistema de notificación. El flujo inicia con el paciente ingresando a la plataforma, seleccionando especialidad, médico y fecha/hora. Luego, el sistema de citas valida la disponibilidad y, si la fecha no está disponible, se notifica al paciente; si está disponible, se registra la cita y se envían los datos al sistema de notificación, que confirma la cita por correo o SMS. Las interacciones se modelaron mediante eventos de mensaje, reflejando una secuencia clara y automatizada del proceso.

- ¿Qué decisiones de modelado se tomaron?

Se decidió utilizar un diagrama BPMN con carriles para representar claramente la responsabilidad de cada actor en el proceso. Se emplearon eventos de mensaje para mostrar la comunicación entre sistemas y compuertas exclusivas para representar decisiones automáticas, como la disponibilidad de citas. Además, se optó por modelar el proceso desde una perspectiva centrada en el paciente, priorizando la claridad del flujo y la automatización de tareas clave.

- ¿Qué herramientas se usaron (papel, pizarra, draw.io, Astah)?

Inicialmente se usó el tablero del salón para establecer los roles principales, actividades e interacciones, lo que le dio un poco de estructura al proceso. Posteriormente se implementó la herramienta draw.io, un software de diagramación que seleccionamos por su facilidad de uso y las opciones de trabajo colaborativo, de manera que se pudiera llevar un proceso de revisión constante entre todos los miembros del equipo.

- ¿Qué parte del trabajo se alcanzó a desarrollar?

Se logró modelar el boceto inicial del proceso de agendamiento de citas médicas, desde el ingreso del paciente a la plataforma hasta la confirmación de la cita por medio del sistema de notificación. Se identificaron los actores involucrados, se definieron sus responsabilidades y se diagramó el flujo principal con sus respectivas decisiones e interacciones.

## 🧩 Boceto inicial del modelo

<img width="1874" height="670" alt="image" src="https://github.com/user-attachments/assets/ad51e775-dba0-493f-b0d0-7e26f0b85c9b" />

Este modelo inicial representa un bosquejo general del proceso de agendamiento de citas médicas, incluyendo las actividades básicas que realiza el paciente (como ingresar a la plataforma, seleccionar especialidad, médico y fecha), y las funciones principales del sistema de citas, como consultar disponibilidad, registrar la cita o notificar la no disponibilidad. También se contempla el envío de confirmación a través del sistema de notificación. 

## 🔁 Tareas definidas para complementar el taller

| Tarea asignada | Responsable | Fecha estimada |
|----------------|-------------|----------------|
| Modelado final en draw.io | Ana Lucía Quintero Vargas | 13/08 |
| Análisis del modelo | Mariana Salas Gutierrez | 14/08 |
| Investigación y referencias | Diego Fernando Ramirez Tenjo | 12/08 |
| Redacción del informe de notas | Carlos Augusto Sánchez Lombana | 12/08 |
|  | Mateo de Jesús Vanegas Correa | 12/08 |
|  | Juan David Cetina Gómez | 12/08 |
---

_Este documento resume el trabajo colaborativo realizado durante la sesión del taller BPMN en el curso AREM - Universidad de La Sabana._