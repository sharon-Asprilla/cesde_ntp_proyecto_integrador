### Parte 2 – Contenido **obligatorio** del archivo README.md

El README **debe** contener **todos** estos apartados en este orden (personalizar el contenido entre corchetes con la información real del grupo). No es opcional ni sugerido; es requisito de evaluación.

```markdown
# [Nombre Oficial del Proyecto]

[knowly]

## Introducción / Contexto

- Descripción del problema que se busca resolver  
- Justificación: ¿por qué es relevante? (impacto social, académico, empresarial, etc.)  
- Breve descripción del dominio / temática del proyecto integrador

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

## Tecnologías y Herramientas (Tech Stack)

- **Frontend**: Streamlit  
- **Backend**: Python  
- **Base de datos**: PostgreSQL  
- **Otras herramientas**: Git, GitHub, Docker, Postman, Swagger

## Integrantes del Equipo

| Nombre                  | Rol principal              | Usuario GitHub     |
|-------------------------|----------------------------|--------------------|
| [Johan Cadavid]         | Líder / Backend            | @[usuario]         |
| [Sebastian Herrera]     | Frontend Lead              | @[usuario]         |
| [Sharon Asprilla]       | Backend / Base de datos    | @[sharon-asprilla] |
| [Juan Jose Castrillon]  | frond/create               | @[usuario]         |
| [Jeronimo Taborda]      | backend                    | @[usuario]         |

## Diagrama de Clases del Dominio (v1)

![Diagrama de Dominio v1](docs/diagrama-dominio-v1.png)  
*Diagrama inicial del modelo de dominio – versión 1. Se actualizará en futuras entregas.*

