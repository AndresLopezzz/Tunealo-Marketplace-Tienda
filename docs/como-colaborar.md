# 📌 Guía de colaboración - Tunealo eCommerce + Marketplace

Este documento explica cómo colaborar en el proyecto usando **Git + GitHub**.

---

## 1. Primeros pasos
1. Acepta la invitación al repositorio en GitHub.
2. Clona el proyecto en tu computadora:

```bash
git clone https://github.com/AndresLopezzz/Tunealo-Marketplace-Tienda.git
cd tunealo-Marketplace-Tienda
```

3. Cambia a la rama `develop` (la usamos como base de trabajo):

```bash
git checkout develop
```

---

## 2. Flujo de trabajo con ramas
👉 Nunca trabajamos directo en `main` ni en `develop`.
Cada tarea debe hacerse en una rama **feature/**.

### Crear una nueva rama para tu tarea
```bash
git checkout develop
git pull origin develop      # actualizar antes de empezar
git checkout -b feature/nombre-tarea
```

Ejemplo:
```bash
git checkout -b feature/login
```

---

## 3. Hacer commits y subir cambios
1. Trabaja en tu código normalmente.
2. Guarda los cambios en Git:

```bash
git add .
git commit -m "feat: agrego pantalla de login con validación básica"
```

3. Sube tu rama al repositorio remoto:

```bash
git push origin feature/login
```

---

## 4. Crear un Pull Request (PR)
1. Ve al repositorio en GitHub.
2. Pestaña **Pull Requests** → **New Pull Request**.
3. Selecciona:
   - Base branch: `develop`
   - Compare branch: `feature/nombre-tarea`
4. Escribe un título y descripción clara.
5. Crea el PR.

---

## 5. Revisión y merge
- Otro compañero o el líder revisará tu PR.
- Si está bien → se aprueba y se hace **merge a `develop`**.
- Si hay cambios → los haces en tu misma rama y haces `git push` de nuevo.

---

## 6. Flujo de ramas

```
feature/*   →   develop   →   testing   →   main
```

- **feature/** → trabajo de cada miembro (login, carrito, admin, etc.)
- **develop** → integración del equipo
- **testing** → pruebas de todo el sistema
- **main** → versión estable para mostrar

---
