# 📝 Guía rápida de Markdown para la documentación

Chuleta con todo lo que necesitas para documentar los temas.

---

## Títulos

```markdown
# Título del documento (solo uno por archivo)
## Sección
### Subsección
```

## Texto

```markdown
**negrita**   *cursiva*   `código en línea`   ~~tachado~~
```

Deja **una línea en blanco** entre párrafos; si no, se juntan.

## Listas

```markdown
- Elemento
- Otro elemento
  - Subelemento (2 espacios de sangría)

1. Paso uno
2. Paso dos
```

## Bloques de código ⭐ (lo más importante)

Tres comillas invertidas (acento grave ` ``` `) y el lenguaje:

````markdown
```bash
php artisan migrate
```

```php
Route::get('/productos', [ProductoController::class, 'index']);
```
````

Lenguajes útiles: `bash`, `php`, `blade`, `html`, `css`, `js`, `sql`, `env`, `json`.

> 💡 Los **comandos** y los **mensajes de error** van SIEMPRE en bloques de código, nunca como capturas: así se pueden copiar y buscar.

## Enlaces

```markdown
[Documentación de Laravel](https://laravel.com/docs)
[Tema 2](tema02-rutas.md)          ← enlace a otro documento del repo
```

## Imágenes / capturas

```markdown
![Texto alternativo que describe la captura](img/tema01/01-pagina-bienvenida.png)
```

Reglas:

1. Guarda la imagen en `docs/img/temaXX/` **dentro del repositorio**.
2. Usa nombres descriptivos, en minúsculas, sin espacios ni tildes y numerados: `01-instalacion-composer.png`, `02-pagina-inicio.png`.
3. La ruta es **relativa** al archivo `.md` (desde `docs/`, la ruta empieza por `img/...`).
4. No arrastres la imagen al editor web de GitHub: se aloja fuera del repositorio.
5. Recorta la captura para mostrar solo lo relevante.

**Atajos para capturas:**

| Sistema | Atajo |
|---------|-------|
| Windows | `Win + Shift + S` |
| macOS | `Cmd + Shift + 4` |
| Linux (GNOME) | `Impr Pant` / `Shift + Impr Pant` |

## Tablas

```markdown
| Comando | Descripción |
|---------|-------------|
| `php artisan serve` | Arranca el servidor de desarrollo |
```

## Citas y avisos

```markdown
> Esto es una cita o una nota.

> [!WARNING]
> Aviso destacado (GitHub lo muestra en color).

> [!TIP]
> Consejo destacado.
```

## Línea separadora

```markdown
---
```

## Casillas de verificación

```markdown
- [x] Hecho
- [ ] Pendiente
```

---

## ✔️ Antes de entregar, comprueba en GitHub

- [ ] Todas las imágenes se ven (si ves un icono roto, revisa la ruta y las mayúsculas/minúsculas).
- [ ] Los bloques de código se ven con colores.
- [ ] Los enlaces del índice del README funcionan.
- [ ] No hay contraseñas ni datos del `.env` en ningún documento ni captura.
