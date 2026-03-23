# level6-7/README.md

# 🧩 Bandit Level 6 → Level 7

## 🎯 Objetivo
La contraseña del siguiente nivel se encuentra en algún lugar del servidor y cumple:
- Pertenece al usuario `bandit7`
- Pertenece al grupo `bandit6`
- Tiene exactamente 33 bytes

---

## 🧠 Problema clave
El archivo no está en el directorio actual y al buscar en todo el sistema aparecen muchos errores de permisos.

---

## 🧠 Conceptos
- `find` → buscar archivos en todo el sistema
- `-user` → filtrar por usuario
- `-group` → filtrar por grupo
- `-size` → tamaño exacto en bytes

---

## 🛠️ Resolución
```bash
find / -type f -user bandit7 -group bandit6 -size 33c
cat /var/lib/dpkg/info/bandit7.password
```

---

## ➡️ Siguiente nivel
```bash
ssh bandit7@bandit.labs.overthewire.org -p 2220
```

---

## 🧠 Nota personal
Los errores "Permission denied" son normales al buscar en todo el sistema.  
No afectan el resultado, ya que el archivo correcto igualmente aparece.

---

## 🧾 Comando + Resultado
```bash
cat /var/lib/dpkg/info/bandit7.password
morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
```
