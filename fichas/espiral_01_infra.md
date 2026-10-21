# Ficha de Sistematización — Espiral 1
## ERP Django · Espiral E1: Infraestructura y Configuración Base
## UTEC Celaya · Técnico en Programación (SEP 3061300006-23)

| Campo | Contenido |
|---|---|
| **Número de espiral** | 1 |
| **Nombre del ciclo** | Infraestructura y Configuración Base |
| **Semanas** | W01 – W03 |
| **Fecha de inicio** | _17_/_09_/_2026_ |
| **Fecha de cierre** | _07_/_10_/_2026_ |
| **Responsable** | [Paulina Ramírez González] |
| **Asesor** | MC. Román Fernando López González |

---

## 1. Objetivo del ciclo

Establecer el entorno de desarrollo portable en USB y desplegar el
proyecto Django base en Render.com, de modo que cualquier avance
posterior tenga una URL pública verificable desde el inicio del proyecto.

---

## 2. Tareas realizadas

| # | Tarea | Estado | Tiempo invertido |
|---|---|---|---|
| 1 | Configurar Python 3.11 embeddable en USB | ✅ | 1:30 h |
| 2 | Instalar pip y virtualenv | ✅ | 1:00 h |
| 3 | Configurar Git Portable | ✅ | 1:00 h |
| 4 | Crear scripts iniciar/finalizar sesión | ✅ | 2:00 h |
| 5 | Crear proyecto Django con 5 apps | ✅ | 2:30 h |
| 6 | Sistema de templates Fable 5 AzulERP | ✅ | 2:30 h |
| 7 | Configurar WhiteNoise y estáticos | ✅ | 1:30 h |
| 8 | Completar settings_prod.py con PostgreSQL | ✅ | 2:00 h |
| 9 | Crear Procfile, Dockerfile, docker-compose.yml | ✅ | 2:30 h |
| 10 | Crear render.yaml | ✅ | 1:00 h |
| 11 | Desplegar en Render.com → URL pública | ✅ | 2:30 h |
| 12 | Ejecutar Sprint 0 Review y Retrospectiva | ✅ | 1:30 h |

---

## 3. Evidencias generadas

- [✅] Repositorio GitHub: `https://github.com/paurmzg/django.git`
- [✅] URL pública Render: `https://django-9osz.onrender.com`
- [✅] Captura de pantalla: `evidencias/espiral_01/render_url.png`
- [✅] Captura de pantalla: `evidencias/espiral_01/manage_check.png`
- [✅] Resultado de tests: `Ran 33 tests in X.XXXs — OK`
- [✅] Commit de cierre: `efd081c (HEAD -> main) Sprint 0 W01: entorno portable + proyecto Django base + 5 apps`


---

## 4. Criterios de aceptación verificados

| Criterio | ¿Cumplido? | Evidencia |
|---|---|---|
| `manage.py check --deploy` sin warnings críticos | ✅ | Captura de terminal |
| URL pública `https://…onrender.com/` → HTTP 200 | ✅ | Captura del navegador |
| Repositorio con ≥ 6 commits en rama `main` | ✅ | `git log --oneline` |
| 33 tests pasando (W01 + W02 + W03) | ✅ | Resultado pytest |
| Ficha Schmelkes E1 completa | ✅ | Este documento |

---

## 5. Problemas encontrados y soluciones

| Problema | Causa | Solución aplicada |
|Configuración del entorno portable|Dependencias no configuradas|Se instaló pip y virtualenv.
| Archivos estáticos no cargaban|Configuración para producción incompleta|Se configuró WhiteNoise. |
| Procesos repetitivos|Falta de automatización |Se crearon scripts de inicio y cierre. |

---

## 6. Lecciones aprendidas

1.Un entorno portable facilita el desarrollo en diferentes equipos.
2.La configuración de producción debe separarse del entorno local.
3.La automatización reduce errores y tareas repetitivas.

---

## 7. Tiempo total invertido

| Categoría | Horas |
| Diseño / planeación | 2h |
| Implementación | 9h |
| Pruebas | 3h |
| Despliegue | 2.5h |
| Documentación | 3.5h |
| **Total Espiral 1** | 20h |

---

## 8. Conexión con el trabajo recepcional

> Esta espiral aporta evidencia para el **Capítulo 4** (Desarrollo),
> sección 4.1 "Espiral 1: Infraestructura", y para el
> **Capítulo 3** (Metodología), subsección "Ciclos del modelo espiral".