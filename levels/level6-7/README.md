# level6-7/README.md

# 🧩 Bandit Level 6 → Level 7

## 🎯 Objetivo
La contraseña del siguiente nivel se encuentra en algún lugar del servidor y cumple:
- Pertenece al usuario `bandit7`
- Pertenece al grupo `bandit6`
- Tiene exactamente 33 bytes

---

## 🧠 Problema clave
El archivo no está en el directorio home y al buscar en todo el sistema aparecen muchos errores de permisos.

---

## 🧠 Conceptos
- `find` → buscar archivos en todo el sistema
- `-user` → filtrar por usuario
- `-group` → filtrar por grupo
- `-size` → tamaño exacto
- `2>/dev/null` → ocultar errores

---

## 🛠️ Resolución
```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
cat /var/lib/dpkg/info/bandit7.password
```

---

## ➡️ Siguiente nivel
```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```

---

## 🧠 Nota personal
Al buscar en todo el sistema aparecen muchos errores de permisos.  
Se pueden ignorar o redirigir a `/dev/null` para ver solo el resultado útil.

---

## 🧾 Comando + Resultado
```bash
cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```
