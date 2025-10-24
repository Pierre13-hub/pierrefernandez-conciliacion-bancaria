# Documento técnico: Migración Bitbucket → GitHub

Este documento describe los pasos realizados para simular la migración de un repositorio técnico desde Bitbucket a GitHub, manteniendo la estructura de ramas, historial de commits y documentación asociada.

---

## 🎯 Objetivo

- Simular una migración completa de repositorio
- Validar trazabilidad entre versiones
- Documentar comandos utilizados y entregables generados

---

## 🗂 Estructura original en Bitbucket

- Repositorio: `conciliacion-bancaria`
- Ramas: `main`, `legacy`, `docs`
- Documentación técnica en `/docs`
- Simulaciones Cobol/RPG en `/src`

---

## 🔄 Comandos utilizados

```bash
# Clonar el repositorio completo con historial
git clone --mirror https://bitbucket.org/usuario/conciliacion-bancaria.git

# Crear repositorio vacío en GitHub

# Subir el mirror completo
cd conciliacion-bancaria.git
git remote add github https://github.com/usuario/conciliacion-bancaria.git
git push --mirror github

