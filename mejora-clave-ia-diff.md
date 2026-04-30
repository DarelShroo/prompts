# 💣 Mejora clave (esto es lo que marca la diferencia)

No te quedes solo en el prompt. Monta este flujo:

## 🧾 1. Genera el diff

```bash
git diff main > diff.txt
```

---

## 📌 2. Añade contexto del commit (MUY IMPORTANTE)

```bash
git show --name-only > commit_context.txt
```

---

## 🌳 3. Estructura del proyecto (si puedes)

```bash
tree -L 3 > structure.txt
```

---

## 🤖 4. Entrada completa a la IA

Le pasas TODO esto junto:

- diff.txt
- commit_context.txt
- structure.txt
- Issue original

---

# 🧠 Idea más avanzada (nivel pro)

Si quieres llevar esto a otro nivel (por ejemplo en Brevio o en tu flujo de trabajo real):

## ⚙️ Automatización completa en un script

- Recoge issue (desde Jira o GitHub)
- Genera diff automáticamente
- Extrae contexto del commit
- Construye el input estructurado
- Llama a la IA
- Genera un reporte en .md

---

## 🚨 Validación automática en CI/CD

Puedes convertir esto en un gate del pipeline:

- Si el análisis devuelve:
  - ❌ Veredicto = "Incorrecto o incompleto"

👉 Entonces el pipeline falla automáticamente

---

## 🧩 Resultado

Esto convierte la IA de:
> “herramienta de ayuda”

a:
> “revisor automático de calidad en CI”
