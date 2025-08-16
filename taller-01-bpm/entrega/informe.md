# 📄 Informe Técnico del Taller

## 🔖 Nombre del Taller
Taller 1 - BPMN

## 👥 Integrantes del equipo
- Ana Lucia Quintero Vargas (anaquiva@unisabana.edu.co)
- Juan David Cetina Gómez (juancego@unisabana.edu.co)
- Carlos Augusto Sánchez Lombana (carlossanlo@unisabana.edu.co)
- Mateo de Jesus Vanegas Correa (mateovaco@unisabana.edu.co)
- Diego Fernández Ramírez Tenjo (diegorate@unisabana.edu.co)
- Mariana Salas Gutiérrez (marianasalgu@unisabana.edu.co)

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
### Buenas prácticas BPMN:
...

### Resumen:
Describa en 2–3 párrafos lo investigado, citando fuentes cuando sea necesario. Incluya cómo se relaciona con el taller.

## 📚 Referencias
- [1] Apellido, Nombre. *Título*. Año. URL o DOI.
- [2] Fuente oficial BPMN: https://www.omg.org/spec/BPMN/

---

_Este documento hace parte de la entrega del taller BPMN del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
