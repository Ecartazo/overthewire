# 🧩 Bandit Level 3 → Level 4

## 🎯 Objetivo
La contraseña del siguiente nivel se encuentra en un archivo oculto dentro del directorio `inhere`.

---

## 🧠 Problema clave
El archivo está oculto. En Linux, los archivos ocultos comienzan con `.` y no se muestran con un `ls` normal.

---

## 🧠 Conceptos
- `ls -a` → muestra archivos ocultos
- `cd` → cambiar de directorio
- `cat` → leer archivos

---

## 🛠️ Resolución
```bash
cd inhere
ls -a
cat ./...Hiding-From-You
```

---

## ➡️ Siguiente nivel
```bash
ssh bandit4@bandit.labs.overthewire.org -p 2220
```

---

## 🧠 Nota personal
Los archivos ocultos en Linux comienzan con `.` y no aparecen con `ls` normal.  
Siempre usar `ls -a` cuando no encontrás algo.

---

## 🧾 Comando + Resultado
```bash
cat ./...Hiding-From-You
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
```
