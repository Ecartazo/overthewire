# level5-6/README.md

# 🧩 Bandit Level 5 → Level 6

## 🎯 Objetivo
La contraseña del siguiente nivel se encuentra en un archivo dentro del directorio `inhere` que cumple:
- Es legible por humanos
- Tiene exactamente 1033 bytes
- No es ejecutable

---

## 🧠 Problema clave
Hay muchos archivos en subdirectorios, por lo que se debe usar `find` para filtrar correctamente.

---

## 🧠 Conceptos
- `find` → buscar archivos
- `-type f` → solo archivos
- `-size 1033c` → tamaño exacto en bytes

---

## 🛠️ Resolución
```bash
cd inhere
find . -type f -size 1033c
cat ./maybehere07/.file2
```

---

## ➡️ Siguiente nivel
```bash
ssh bandit6@bandit.labs.overthewire.org -p 2220
```

---

## 🧠 Nota personal
Filtrar por tamaño con `find` es la forma más rápida de encontrar archivos específicos.

---

## 🧾 Comando + Resultado
```bash
cat ./maybehere07/.file2
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
```
