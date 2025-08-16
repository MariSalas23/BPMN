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
Explique cómo realizaron el trabajo: qué decisiones tomaron, qué herramientas utilizaron, qué aspectos modelaron primero y cómo lo fueron ajustando.

## 🧩 Análisis del modelo propuesto
Incluya un análisis sobre:
- ¿Cómo se estructura el modelo entregado?
- ¿Cómo representa las necesidades del cliente?
- ¿Qué supuestos se tomaron?

## 📈 Diagrama final entregado
Enlace al modelo final: https://drive.google.com/file/d/1BJv5aFeUThF4R61ce-uZ2SmcK3yexryq/view?usp=sharing

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
