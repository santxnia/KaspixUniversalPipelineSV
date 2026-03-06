# Guía: Crear el Repositorio en GitHub

Sigue estos pasos para subir el pipeline a GitHub.

## 1. Crear el repo en GitHub

1. Ve a https://github.com/new
2. Nombre del repositorio: `kaspix-universal-pipeline`
3. Descripción: `Pipeline universal para generación de gemelos digitales de componentes Analog Devices`
4. Visibilidad: **Public**
5. ❌ NO inicialices con README (ya tienes uno)
6. Clic en **Create repository**

---

## 2. Subir los archivos locales

Desde la carpeta del proyecto en tu máquina:

```bash
git init
git add .
git commit -m "feat: initial commit - estructura base del pipeline"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/kaspix-universal-pipeline.git
git push -u origin main
```

---

## 3. Flujo de trabajo recomendado para avances

Cada vez que avances en el proyecto:

```bash
# Ver qué cambió
git status

# Agregar cambios
git add .

# Commit descriptivo
git commit -m "feat: descripción del avance"

# Subir
git push
```

### Convención de commits sugerida:
| Prefijo | Uso |
|---------|-----|
| `feat:` | Nueva funcionalidad o módulo |
| `fix:` | Corrección de bug |
| `docs:` | Cambios en documentación |
| `refactor:` | Reestructuración de código |
| `wip:` | Trabajo en progreso |

---

## 4. Branches recomendados

```bash
main          # versión estable
dev           # desarrollo activo
feature/xxx   # módulos específicos
```
