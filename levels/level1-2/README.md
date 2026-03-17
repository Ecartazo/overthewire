# 🧩 Bandit Level 1 → Level 2

## 🎯 Objetivo
La contraseña del siguiente nivel se encuentra en un archivo llamado `-` dentro del directorio home.

---

## 🧠 Problema clave

El archivo se llama `-`, lo cual en Linux es un carácter especial que suele representar la entrada estándar (stdin).  
Por eso, no se puede leer de forma directa con `cat -`.

---

## 🧠 Conceptos
- `ls` → listar archivos
- `cat` → leer archivos
- Uso de `./` para manejar nombres especiales

---

## 🛠️ Resolución

Listamos los archivos:

```bash
ls
bandit1@bandit:~$ cat ./-
263JGJPfgU6LtdEvgfWU1XP5yac29mFx
