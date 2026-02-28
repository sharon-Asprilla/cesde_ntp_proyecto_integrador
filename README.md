### Parte 2 – Contenido **obligatorio** del archivo README.md

El README **debe** contener **todos** estos apartados en este orden (personalizar el contenido entre corchetes con la información real del grupo). No es opcional ni sugerido; es requisito de evaluación.

```markdown
# [Nombre Oficial del Proyecto]

[knowly]

## Introducción / Contexto

- Descripción del problema que se busca resolver  

En la actualidad, muchas personas buscan aprender de manera independiente y flexible, mientras que profesores y expertos desean compartir sus conocimientos y generar ingresos adicionales. Sin embargo, existen limitaciones como por ejemplo las plataformas son muy costosas, e incluso carecen de material de estudio, las personas que realizan los cursos no tiene como esa credencialidad del certificado


- Justificación: ¿por qué es relevante? (impacto social, académico, empresarial, etc.)  

Desarrollar una plataforma local (que siempre que este conectada al internet pueda  funcionar si no no deja ingresar) con tal de que los estudiantes puedan acceder en cualquier lugar y hora en el mundo  y sus estudios se llevan de  forma independiente, ademas los profesores  generan ingresos y comparten conocimientos

- Breve descripción del dominio / temática del proyecto integrador


es hacer una plataforma donde la monetizacion directa y el aprendizaje independiente, por lo cual las personas pagan suscripcion por algo esclusivo, cada curso tiene su certificado y se puede tener fors y hacer comentarios he incluso tener un chat con el profesor donde las preguntas se pueden ver, no solo el profe si no los otros usuarios, ademas pueden subir actividades realizadas y hacer un examen 

## Objetivos

**Objetivo General**  
[Redactar el objetivo general del proyecto integrador – una frase clara y concreta]

**Objetivos Específicos**  
- [OE1 – descripción clara]  
- [OE2 – descripción clara]  
- [OE3 – descripción clara]  
- [OE4 – descripción clara]  
(Mínimo 3–5 objetivos específicos)

## Alcance del Proyecto (Scope)

**Qué se va a desarrollar:**  
- [Listar módulos principales y funcionalidades clave previstas en el semestre]

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


