### Parte 2 – Contenido **obligatorio** del archivo README.md

El README **debe** contener **todos** estos apartados en este orden (personalizar el contenido entre corchetes con la información real del grupo). No es opcional ni sugerido; es requisito de evaluación.

```markdown
# [knowly]

knowly es una plataforma donde las personas pueden aprender a su ritmo de forma virtual

## Introducción / Contexto

- Descripción del problema que se busca resolver  

En la actualidad, muchas personas buscan aprender de manera independiente y flexible, mientras que profesores y expertos desean compartir sus conocimientos y generar ingresos adicionales. Sin embargo, existen limitaciones como por ejemplo las plataformas son muy costosas, e incluso carecen de material de estudio, las personas que realizan los cursos no tiene como esa credencialidad del certificado


- Justificación: ¿por qué es relevante? (impacto social, académico, empresarial, etc.)  

Desarrollar una plataforma local (que siempre que este conectada al internet pueda  funcionar si no no deja ingresar) con tal de que los estudiantes puedan acceder en cualquier lugar y hora en el mundo  y sus estudios se llevan de  forma independiente, ademas los profesores  generan ingresos y comparten conocimientos

- Breve descripción del dominio / temática del proyecto integrador


es hacer una plataforma donde la monetizacion directa y el aprendizaje independiente, por lo cual las personas pagan suscripcion por algo esclusivo, cada curso tiene su certificado y se puede tener fors y hacer comentarios he incluso tener un chat con el profesor donde las preguntas se pueden ver, no solo el profe si no los otros usuarios, ademas pueden subir actividades realizadas y hacer un examen 

## Objetivos

**Objetivo General**  
[Diseñar y desarrollar una plataforma digital integral que permita la creación, gestión y monetización de comunidades en línea, proporcionando a los creadores herramientas intuitivas y escalables para organizar contenidos, fomentar la interacción activa y construir relaciones sostenibles con sus usuarios, al mismo tiempo que se garantiza una experiencia participativa, segura y personalizada para los miembros, impulsando así la generación de valor económico, social y creativo dentro del ecosistema digital.]

**Objetivos Específicos**  
- [OE1 – descripción clara]  
- [OE2 – descripción clara]  
- [OE4 – descripción clara - Implementar un sistema que divida los cursos en categorías (cortos, medianos y largos) para facilitar la búsqueda y selección según el tiempo disponible del usuario.]  
- [OE5 - Incorporar calificaciones y comentarios de los estudiantes para cada curso y profesor, garantizando transparencia y confianza en la calidad del contenido]
- [OE1 – Implementar una plataforma de gestión de aprendizaje (LMS) que permita la reproducción de contenidos multimedia y  el seguimiento del progreso académico del estudiante de forma automatizada.]  
- [OE2 – Crear una interfaz intuitiva y responsiva que facilite la navegación, permitiendo que la compra y el inicio de un curso se realicen de manera fluida en pocos pasos.]  
- [OE3 – Desarrollar un módulo de gestión de pagos que habilite a los profesores la publicación de contenidos previo pago de una tarifa de suscripción o derecho de piso en la plataforma.]   
- [OE4 – descripción clara]  
(Mínimo 3–5 objetivos específicos)

## Alcance del Proyecto (Scope)

**Qué se va a desarrollar:**  
1. Módulo de Gestión de Cuentas y Perfiles
Este módulo permitirá a los usuarios administrar su identidad y seguridad dentro de la plataforma.
• Gestión de perfil: Personalización de nombre, foto de perfil y ubicación en el mapa.
• Seguridad y acceso: Funciones para restablecer contraseñas, cambiar el correo electrónico asociado y cerrar sesión en todos los dispositivos.
• Preferencias de comunicación: Control de notificaciones y ajustes de disponibilidad en el chat.
2. Módulo de Interacción y Comunidad
Se enfoca en las herramientas de comunicación y las reglas de convivencia entre miembros.
• Skool Chat: Sistema de mensajería interna con opciones para bloquear usuarios si es necesario.
• Moderación y seguridad comunitaria: Herramientas para reportar contenido o usuarios, y acceso a las reglas específicas de cada grupo.
• Soporte técnico: Acceso a un centro de ayuda y contacto directo con administradores o soporte vía correo electrónico.
3. Módulo de Gamificación y Participación
Diseñado para incentivar la actividad de los usuarios mediante sistemas de recompensa.
• Sistema de progresión: Implementación de puntos y niveles para los miembros.
• Seguimiento de actividad: Visualización de la actividad diaria del usuario en la plataforma.
4. Módulo de Gestión de Contenidos y Eventos
Administra el acceso a los recursos educativos o sociales del grupo.
• Control de acceso: Funcionalidad para desbloquear cursos o eventos específicos según el progreso o permisos del usuario.
5. Módulo de Pagos y Suscripciones
Permite la gestión financiera tanto para miembros como para administradores.
• Administración de membresías: Opciones para cambiar de plan, cancelar suscripciones y ver el historial de pagos.
• Pasarela de pagos: Actualización de métodos de pago (tarjetas) y gestión de reembolsos.
• Monetización: Sistema para gestionar cuentas bancarias para cobros y programas de referidos con comisiones de afiliado.

**Qué NO se va a desarrollar en esta versión (fuera de alcance):**  
-[incorporacion de api de gemini ya que  esta plataforma evalua mediante al examen final]
-[que la IA no evalue ala persona de manersa didactica, ya que el examen es el que te otorga certificado y cedencialidad]
-[todavia no teiene funcionalidades para traducir el video y cambiarlo de idioma a no ser que sean subtitulo ]


## Tecnologías y Herramientas (Tech Stack)

- **Frontend**: Streamlit  
- **Backend**: Python  
- **Base de datos**: PostgreSQL  
- **Otras herramientas**: Git, GitHub, Docker, Postman, Swagger

## Integrantes del Equipo

| Nombre                  | Rol principal              | Usuario GitHub     |
|-------------------------|----------------------------|--------------------|
| [Johan Cadavid]         | Líder / Backend            | @[usuario]         |
| [Sebastian Herrera]     | Frontend Lead              | @[Sebasherrera01]         |
| [Sharon Asprilla]       | Backend / Base de datos    | @[sharon-asprilla] |
| [Juan Jose Castrillon]  | frond/create               | @[usuario]         |
| [Jeronimo Taborda]      | backend                    | @[usuario]         |

## Diagrama de Clases del Dominio (v1)

![Diagrama de Dominio v1](pages\images\Captura de pantalla 2026-02-28 100147.png)  
*Diagrama inicial del modelo de dominio – versión 1. Se actualizará en futuras entregas.*


    USUARIO {
        int id_usuario PK
        varchar (80) nombre
        varchar (80) apellido
        varchar (10)documento
        varchar (250)correo
        int (8)contraseña
    }

    CURSO {
        int id_curso PK
        varchar (250) nombre_curso
        text (350) descripcion
        float (10,0) precio
        varchar (90) intensidad
    }

    INSCRIPCION {
        int id_inscripcion PK
        int id_usuario FK
        int id_curso FK
        date fecha_inscripcion
    }

    CERTIFICADO {
        int id_certificado PK
        int id_usuario FK
        int id_curso FK
        date fecha_emision
    }

    USUARIO ||--o{ INSCRIPCION : "realiza"}
    CURSO  ||--o{ INSCRIPCION : "tiene"}
    USUARIO ||--o{ CERTIFICADO : "obtiene"}
    CURSO  ||--o{ CERTIFICADO : "otorga"}


