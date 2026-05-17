# ClinicaApp — Sistema de Gestión de Turnos Médicos

Aplicación de consola desarrollada en Java con principios de Programación Orientada a Objetos, como proyecto del Hackathon de Generation Colombia 2026.

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Generation](https://img.shields.io/badge/Hackathon-Generation%20Colombia-red?style=for-the-badge)

---

## Descripción

ClinicaApp permite gestionar pacientes, médicos y turnos de una clínica desde la consola. Los datos se mantienen en memoria durante la sesión y se persisten en archivos CSV al salir, garantizando que la información sobreviva entre ejecuciones.

---

## Funcionalidades

- Registrar pacientes y médicos
- Asignar, cancelar y cambiar el estado de turnos
- Listar turnos del día, por médico o por paciente
- Listar pacientes y médicos ordenados alfabéticamente

---

## Estructura del proyecto

```
clinicaapp/
└── src/
    └── co/generation/clinica/
        ├── model/
        │   ├── Paciente.java
        │   ├── Medico.java
        │   ├── Turno.java
        │   ├── EstadoTurno.java
        │   └── Especialidad.java
        ├── interfaces/
        │   ├── Registrable.java
        │   └── Consultable.java
        ├── service/
        │   └── ClinicaService.java
        ├── datos/
        │   └── DatosCSV.java
        └── Main.java
```

---

## Conceptos OOP aplicados

- **Encapsulamiento** — atributos privados con getters y setters validados
- **Interfaces** — `Registrable` y `Consultable` como contratos de comportamiento
- **Enumeraciones** — `EstadoTurno` y `Especialidad` para valores controlados
- **Equals y HashCode** — sobrescritos para detección de duplicados y conflictos de agenda
- **Persistencia** — serialización y deserialización manual con archivos CSV

---

## Cómo correr el proyecto

**Requisitos:** Java 17 o superior, IntelliJ IDEA

1. Clona el repositorio
```bash
git clone https://github.com/fabian1031/Sistema-de-Gestion-de-Turnos-.git
```
2. Abre IntelliJ IDEA → `File` → `Open` → selecciona la carpeta `clinicaapp/`
3. Clic derecho sobre `src/` → **Mark Directory as** → **Sources Root**
4. Abre `Main.java` y haz clic en **Run**

> Los archivos CSV se generan automáticamente en una carpeta `datos/` la primera vez que ejecutas el programa.

---

## Autor

**Fabian Beltran**

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/fabian1031)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fabian-andres-beltran-vargas-desarrollador-backend/)[https://www.linkedin.com/in/fabian-andres-beltran-vargas-desarrollador-backend/](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](#)