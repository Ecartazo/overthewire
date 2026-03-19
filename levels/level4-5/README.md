# level4-5/README.md

# 🧩 Bandit Level 4 → Level 5

## 🎯 Objetivo
La contraseña del siguiente nivel se encuentra en el único archivo legible por humanos dentro del directorio `inhere`.

---

## 🧠 Problema clave
Hay múltiples archivos, pero solo uno es texto legible.

---

## 🧠 Conceptos
- `file` → identifica tipo de archivo
- `cat` → leer archivos
- `./*` → todos los archivos del directorio

---

## 🛠️ Resolución
```bash
cd inhere
file ./*
cat ./-file07
```

---

## ➡️ Siguiente nivel
```bash
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

---

## 🧠 Nota personal
El comando `file` permite detectar cuál archivo es texto (ASCII).

---

## 🧾 Comando + Resultado
```bash
cat ./-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
```
