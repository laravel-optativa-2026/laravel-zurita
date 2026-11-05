# 📘 Proyecto Laravel — [Tu nombre y apellidos]

> **Curso:** [Curso / Grupo] · **Módulo:** [Nombre del módulo] · **Curso académico:** 20XX-20XX

Este repositorio contiene la aplicación Laravel que estoy desarrollando siguiendo los temas de autoformación, junto con la documentación de cada tema: pasos seguidos, comandos empleados, capturas de pantalla, problemas encontrados y cómo los he resuelto.

---

## 📂 Estructura del repositorio

```
├── README.md              ← Esta portada (índice de temas)
├── proyecto/              ← Aplicación Laravel
├── docs/
│   ├── PLANTILLA-TEMA.md  ← Plantilla: cópiala para cada tema nuevo
│   ├── GUIA-MARKDOWN.md   ← Chuleta de Markdown
│   ├── temaXX-nombre.md   ← Documentación de cada tema
│   └── img/
│       └── temaXX/        ← Capturas de cada tema
└── .github/
    └── pull_request_template.md
```

---

## 📑 Índice de temas

| Tema | Título | Estado |
|:----:|--------|:------:|
| 01 | [Instalación y primer proyecto](docs/tema01-instalacion.md) | ⏳ |
| 02 | [Título del tema 2](docs/tema02-nombre.md) | ⏳ |
| 03 | [Título del tema 3](docs/tema03-nombre.md) | ⏳ |

> Estados: ⏳ pendiente · 🚧 en curso · ✅ terminado · 🔁 corregido tras revisión

---

## 🔑 Primera vez: acceder al repositorio

1. Acepta la invitación que te ha llegado por correo (o en <https://github.com/notifications>).
2. Clona el repositorio en tu equipo (copia la URL del botón verde **Code**):
   ```bash
   git clone https://github.com/ORGANIZACION/laravel-tu-usuario.git
   cd laravel-tu-usuario
   ```

> ℹ️ La rama `main` está protegida: **no puedes subir cambios directamente a ella**. Todo el trabajo se hace en una rama por tema y llega a `main` mediante un Pull Request que el profesor debe aprobar.

---

## 🚀 Cómo trabajar cada tema

1. **Actualiza tu repositorio y crea la rama del tema:**
   ```bash
   git checkout main
   git pull
   git checkout -b tema01
   ```
2. **Crea el documento del tema** copiando la plantilla:
   ```bash
   cp docs/PLANTILLA-TEMA.md docs/tema01-instalacion.md
   mkdir -p docs/img/tema01
   ```
3. **Trabaja y documenta a la vez.** No dejes la documentación para el final: copia los comandos y los errores en el momento en que aparecen.
4. **Haz commits frecuentes** con mensajes claros:
   ```bash
   git add .
   git commit -m "Tema 1: instalación de Laravel y configuración del .env"
   git push -u origin tema01
   ```
5. **Al terminar, abre un Pull Request** de `tema01` hacia `main` en GitHub y revisa la checklist que aparece automáticamente.
6. **Corrige lo que te indique el profesor** en los comentarios del Pull Request (nuevos commits en la misma rama). Cuando esté aprobado, pulsa **Merge pull request**. Si subes cambios después de la aprobación, tendrá que volver a aprobarlo.
7. **Actualiza el estado del tema** en el índice de este README.

---

## ⚙️ Primera vez: crear el proyecto Laravel

El proyecto Laravel va dentro de la carpeta `proyecto/` (hazlo ya en la rama `tema01`):

```bash
# Desde la raíz del repositorio, en la rama tema01
rm proyecto/.gitkeep
composer create-project laravel/laravel proyecto
cd proyecto
php artisan serve
```

> ⚠️ **Nunca subas el archivo `.env`** ni la carpeta `vendor/`. El `.gitignore` de Laravel ya los excluye; no lo modifiques.

Para poner en marcha el proyecto tras clonarlo en otro equipo:

```bash
cd proyecto
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```
