# 📚 **GUÍA COMPLETA: Comandos de Git y GitHub**

## **⚙️ GIT - COMANDOS PRINCIPALES**

### **🏁 CONFIGURACIÓN INICIAL**
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```
**¿Qué es?** Configura tu identidad para todos los commits  
**Para qué sirve:** Identifica quién hace cada cambio  
**Herramientas:** Terminal, Git Bash, CMD

---

### **📁 INICIALIZACIÓN Y CLONACIÓN**
```bash
git init
```
**¿Qué es?** Crea un nuevo repositorio local  
**Para qué sirve:** Comenzar a trackear cambios en un proyecto  
**Cuándo usarlo:** Al empezar un proyecto nuevo

```bash
git clone https://github.com/usuario/repositorio.git
```
**¿Qué es?** Copia un repositorio remoto a local  
**Para qué sirve:** Obtener código existente de GitHub

**Herramientas:** Terminal, GitHub Desktop, GitKraken

---

### **📊 ESTADO Y SEGUIMIENTO**
```bash
git status
```
**¿Qué es?** Muestra el estado actual del repositorio  
**Para qué sirve:** Ver archivos modificados, añadidos, eliminados  
**Herramientas:** Terminal, GitKraken (interfaz visual)

```bash
git add nombre-archivo
git add .
git add -A
```
**¿Qué es?** Añade archivos al "staging area"  
**Para qué sirve:** Preparar cambios para el commit  
**Diferencia:**
- `add .` → archivos nuevos y modificados
- `add -A` → todos los cambios incluyendo eliminados

---

### **💾 GUARDAR CAMBIOS**
```bash
git commit -m "Mensaje descriptivo"
```
**¿Qué es?** Guarda los cambios del staging en el historial  
**Para qué sirve:** Crear puntos de restauración  
**Herramientas:** Terminal, VS Code (extensión Git)

```bash
git commit --amend
```
**¿Qué es?** Modifica el último commit  
**Para qué sirve:** Corregir mensajes o añadir archivos olvidados

---

### **📚 HISTORIAL Y COMPARACIÓN**
```bash
git log
git log --oneline
git log --graph
```
**¿Qué es?** Muestra el historial de commits  
**Para qué sirve:** Ver evolución del proyecto  
**Herramientas:** GitKraken (timeline visual), GitHub Desktop

```bash
git diff
git diff nombre-archivo
```
**¿Qué es?** Muestra diferencias entre versiones  
**Para qué sirve:** Ver qué cambió exactamente

---

### **🌿 TRABAJO CON RAMAS**
```bash
git branch nombre-rama
```
**¿Qué es?** Crea una nueva rama  
**Para qué sirve:** Desarrollo paralelo sin afectar main

```bash
git checkout nombre-rama
git switch nombre-rama
```
**¿Qué es?** Cambia entre ramas  
**Para qué sirve:** Moverse entre líneas de desarrollo

```bash
git merge nombre-rama
```
**¿Qué es?** Fusiona ramas  
**Para qué sirve:** Incorporar cambios de una rama a otra

**Herramientas:** GitKraken (arrastrar y soltar), GitHub Desktop

---

### **🔄 SINCRONIZACIÓN CON REMOTO**
```bash
git push origin main
```
**¿Qué es?** Envía commits locales al repositorio remoto  
**Para qué sirve:** Compartir cambios con el equipo

```bash
git pull origin main
```
**¿Qué es?** Obtiene cambios del remoto y los fusiona  
**Para qué sirve:** Actualizar repositorio local

```bash
git fetch
```
**¿Qué es?** Descarga cambios pero no fusiona  
**Para qué sirve:** Ver qué hay nuevo sin modificar tu trabajo

---

## **🌐 GITHUB - FUNCIONALIDADES PRINCIPALES**

### **📋 PULL REQUESTS**
**¿Qué es?** Solicitud para fusionar cambios  
**Para qué sirve:** Revisión de código antes de integrar  
**Herramientas:** Interfaz web de GitHub, GitHub CLI

### **🎫 ISSUES**
**¿Qué es?** Sistema de reporte de bugs y características  
**Para qué sirve:** Seguimiento de tareas y problemas  
**Herramientas:** Interfaz web, integración con proyectos

### **🔀 FORKS**
**¿Qué es?** Copia personal de un repositorio  
**Para qué sirve:** Contribuir a proyectos sin acceso de escritura

---

## **🛠️ HERRAMIENTAS POR CATEGORÍA**

### **TERMINAL/CLI**
- **Git Bash** (Windows)
- **Terminal** (macOS/Linux)
- **Windows PowerShell**
- **GitHub CLI** (`gh` command)

### **INTERFACES GRÁFICAS**
- **GitHub Desktop** - Ideal para principiantes
- **GitKraken** - Muy visual y poderosa
- **SourceTree** - Completa y gratuita
- **VS Code Git Extension** - Integrada en el editor

### **EXTENSIONES Y ADD-ONS**
- **GitLens** (VS Code) - Mejora visualización Git
- **Git Graph** (VS Code) - Timeline visual
- **GitHub Pull Requests** (VS Code)

---

## **🔄 FLUJO DE TRABAJO COMBINADO**

### **ESCENARIO TÍPICO:**
```bash
# 1. Actualizar local
git pull origin main

# 2. Crear rama para nueva feature
git checkout -b feature/nueva-funcionalidad

# 3. Trabajar y guardar cambios
git add .
git commit -m "Añadir nueva funcionalidad"

# 4. Subir al remoto
git push origin feature/nueva-funcionalidad

# 5. En GitHub: crear Pull Request
# 6. Después del merge: limpiar
git checkout main
git pull origin main
git branch -d feature/nueva-funcionalidad
```

### **HERRAMIENTAS PARA CADA ETAPA:**

| **Etapa**     | **Git Command** | **Herramienta GUI** |
|---------------|-----------------|---------------------|
| Configuración | `git config`    | GitHub Desktop      |
| Clonación     | `git clone`     | GitKraken           |
| Staging       | `git add`       | VS Code Source Control |
| Commits       | `git commit`    | GitHub Desktop      |
| Ramas         | `git branch`    | GitKraken Graph     |
| Merge         | `git merge`     | GitHub Pull Requests|
| Sincronización| `git push/pull` | GitHub Desktop Sync |

---

## **🔗 ENLACES A HERRAMIENTAS**

- **📥 Git Official**: https://git-scm.com/
- **🐙 GitHub**: https://github.com/
- **🖥️ GitHub Desktop**: https://desktop.github.com/
- **🐙 GitKraken**: https://www.gitkraken.com/
- **🌳 SourceTree**: https://www.sourcetreeapp.com/
- **👁️ GitLens**: https://gitlens.amod.io/
- **📊 Git Graph**: Extensión VS Code