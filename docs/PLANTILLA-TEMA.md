# Tema XX: [Título del tema]

| | |
|---|---|
| **Fecha de inicio** | dd/mm/aaaa |
| **Fecha de fin** | dd/mm/aaaa |
| **Tiempo dedicado** | X horas |
| **Rama de Git** | `temaXX` |

---

## 1. 🎯 Objetivo del tema

<!-- Explica con TUS palabras qué había que conseguir en este tema (2-4 líneas).
     No copies el enunciado. -->

---

## 2. 🛠️ Desarrollo paso a paso

<!-- Un apartado por cada paso importante. Para cada uno:
     - Qué haces y POR QUÉ.
     - El comando o el código, en un bloque de código (nunca como captura).
     - Una captura solo si aporta algo visual (navegador, resultado, estructura...). -->

### 2.1 [Nombre del paso]

Explicación de lo que hago y para qué sirve.

```bash
php artisan make:model Producto -m
```

Fragmento de código relevante (indica el archivo):

```php
// proyecto/app/Models/Producto.php
class Producto extends Model
{
    protected $fillable = ['nombre', 'precio'];
}
```

![Descripción de la captura](img/temaXX/01-descripcion.png)

### 2.2 [Nombre del paso]

...

---

## 3. 📋 Resumen de comandos utilizados

| Comando | Para qué sirve |
|---------|----------------|
| `php artisan ...` | ... |
| `composer ...` | ... |
| `git ...` | ... |

---

## 4. 🐞 Problemas encontrados y soluciones

<!-- Documenta TODOS los problemas, aunque te parezcan tontos.
     Copia el error como texto, no como captura.
     Si no has tenido ningún problema, documenta al menos algo que hayas tenido que investigar. -->

### Problema 1: [Descripción corta]

**Qué estaba haciendo:** ...

**Error:**

```
Pega aquí el mensaje de error completo
```

**Causa:** por qué ocurría (lo que has entendido, no solo lo que has hecho).

**Solución:**

```bash
comando o cambio que lo resolvió
```

**Fuente:** [enlace a la documentación, foro, vídeo...](https://)

### Problema 2: [Descripción corta]

...

---

## 5. ✅ Resultado final

<!-- Captura(s) de la aplicación funcionando al terminar el tema. -->

![Resultado final del tema](img/temaXX/99-resultado-final.png)

---

## 6. 💭 Conclusiones

- **Qué he aprendido:** ...
- **Qué me ha costado más:** ...
- **Qué haría diferente / dudas pendientes:** ...
