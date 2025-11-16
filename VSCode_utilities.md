# 🚀 **SNIPPETS Y SHORTCUTS COMPLETOS DE VS CODE**

## **⌨️ SHORTCUTS ESENCIALES (WINDOWS/LINUX)**

### **📁 ARCHIVOS Y NAVEGACIÓN**
```typescript
Ctrl + N                    // Nuevo archivo
Ctrl + O                    // Abrir archivo
Ctrl + S                    // Guardar
Ctrl + Shift + S           // Guardar como
Ctrl + K S                 // Guardar todos
Ctrl + W                   // Cerrar pestaña
Ctrl + Shift + T           // Reabrir pestaña cerrada
Ctrl + Tab                 // Cambiar entre pestañas
Ctrl + P                   // Buscar archivo por nombre
```

### **🎯 EDITOR DE TEXTO**
```typescript
Ctrl + C                   // Copiar línea
Ctrl + X                   // Cortar línea
Ctrl + V                   // Pegar
Ctrl + Z                   // Deshacer
Ctrl + Y                   // Rehacer
Ctrl + D                   // Seleccionar siguiente coincidencia
Ctrl + Shift + L           // Seleccionar todas las coincidencias
Alt + ↑/↓                  // Mover línea arriba/abajo
Ctrl + Shift + K           // Eliminar línea
Ctrl + /                   // Comentar/descomentar línea
Ctrl + Shift + /           // Comentar bloque
```

### **🔍 BUSCAR Y REEMPLAZAR**
```typescript
Ctrl + F                   // Buscar en archivo
Ctrl + H                   // Reemplazar en archivo
Ctrl + Shift + F           // Buscar en todos los archivos
Ctrl + Shift + H           // Reemplazar en todos los archivos
F3                         // Siguiente resultado
Shift + F3                 // Anterior resultado
```

### **🌿 CONTROL DE VERSIONES (GIT)**
```typescript
Ctrl + Shift + G           // Panel de Git
Ctrl + Enter               // Confirmar cambios
Alt + ↑/↓                  // Navegar entre cambios
Ctrl + Shift + P, git      // Comandos de Git
```

---

## **🖥️ SHORTCUTS PARA MAC**
```typescript
Cmd + N                    // Nuevo archivo
Cmd + O                    // Abrir archivo
Cmd + S                    // Guardar
Cmd + Shift + S           // Guardar como
Cmd + W                   // Cerrar pestaña
Cmd + Tab                 // Cambiar entre apps
Cmd + P                   // Buscar archivo
Cmd + D                   // Seleccionar siguiente coincidencia
Cmd + /                   // Comentar línea
```

---

## **⚡ SNIPPETS PERSONALIZADOS**

### **📝 CREAR SNIPPETS GLOBALES**
1. **Ctrl + Shift + P**
2. **"Preferences: Configure User Snippets"**
3. **Selecciona el lenguaje o "Global"**

### **🔧 EJEMPLOS DE SNIPPETS ÚTILES**

**Para JavaScript/TypeScript:**
```json
{
  "Console Log": {
    "prefix": "cl",
    "body": [
      "console.log('$1:', $1);",
      "$2"
    ],
    "description": "Console log variable"
  },
  "Function Component": {
    "prefix": "rfc",
    "body": [
      "import React from 'react';",
      "",
      "const ${1:Component} = () => {",
      "  return (",
      "    <div>",
      "      $2",
      "    </div>",
      "  );",
      "};",
      "",
      "export default ${1:Component};"
    ]
  }
}
```

**Para HTML:**
```json
{
  "HTML5 Base": {
    "prefix": "html5",
    "body": [
      "<!DOCTYPE html>",
      "<html lang=\"en\">",
      "<head>",
      "  <meta charset=\"UTF-8\">",
      "  <meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">",
      "  <title>$1</title>",
      "</head>",
      "<body>",
      "  $2",
      "</body>",
      "</html>"
    ]
  }
}
```

**Para Python:**
```json
{
  "Main Function": {
    "prefix": "main",
    "body": [
      "if __name__ == \"__main__\":",
      "    $1"
    ]
  },
  "Print Debug": {
    "prefix": "pd",
    "body": [
      "print(f\"${1:variable}: {${1:variable}}\")"
    ]
  }
}
```

---

## **🎨 SNIPPETS PARA GIT**

### **COMMIT MESSAGES CONVENCIONALES**
```json
{
  "Git Commit Feat": {
    "prefix": "gfeat",
    "body": [
      "feat: $1"
    ]
  },
  "Git Commit Fix": {
    "prefix": "gfix",
    "body": [
      "fix: $1"
    ]
  },
  "Git Commit Docs": {
    "prefix": "gdocs",
    "body": [
      "docs: $1"
    ]
  }
}
```

---

## **🚀 PRODUCTIVIDAD AVANZADA**

### **MULTI-CURSOR**
```typescript
Ctrl + Alt + ↑/↓          // Agregar cursor arriba/abajo
Ctrl + U                  // Deshacer última operación cursor
Shift + Alt + I           // Agregar cursor al final de cada línea
Ctrl + Shift + L          // Seleccionar todas las ocurrencias
```

### **NAVEGACIÓN RÁPIDA**
```typescript
Ctrl + G                  // Ir a línea
Ctrl + Shift + O          // Ir a símbolo en archivo
Ctrl + T                  // Ir a símbolo en workspace
F12                       // Ir a definición
Alt + F12                 // Ver definición
Ctrl + K F12              // Abrir definición al lado
```

### **TERMINAL INTEGRADO**
```typescript
Ctrl + `                  // Abrir/cerrar terminal
Ctrl + Shift + `          // Nuevo terminal
Ctrl + Shift + C          // Abrir terminal externo
Ctrl + C                  // Copiar en terminal
Ctrl + V                  // Pegar en terminal
```

---

## **🔧 SNIPPETS PARA CSS/TAILWIND**

```json
{
  "Flex Center": {
    "prefix": "flexc",
    "body": [
      "display: flex;",
      "justify-content: center;",
      "align-items: center;"
    ]
  },
  "Grid Center": {
    "prefix": "gridc",
    "body": [
      "display: grid;",
      "place-items: center;"
    ]
  },
  "Tailwind Container": {
    "prefix": "twcont",
    "body": [
      "className=\"container mx-auto px-4\""
    ]
  }
}
```

---

## **📦 EXTENSIONES QUE AGREGAN SNIPPETS ÚTILES**

### **ES7+ REACT/REDUX/GRAPHQL**
- `rafc` → Arrow function component
- `rfce` → Functional component export
- `rcc` → Class component

### **AUTO IMPORT**
- Importa automáticamente dependencias

### **THUNDER CLIENT** (REST API)
- Snippets para testing APIs

### **GITLENS**
- `#` → Insertar commit hash
- `@` → Mención de usuario

---

## **🎯 MIS SNIPPETS PERSONALES FAVORITOS**

### **REACT HOOKS**
```json
{
  "UseState": {
    "prefix": "us",
    "body": [
      "const [${1:state}, set${1/(.*)/${1:/capitalize}/}] = useState(${2:initialValue});"
    ]
  },
  "UseEffect": {
    "prefix": "ue",
    "body": [
      "useEffect(() => {",
      "  $1",
      "}, [${2:dependencies}]);"
    ]
  }
}
```

### **DEBUGGING**
```json
{
  "Debug Block": {
    "prefix": "debug",
    "body": [
      "console.log('=== DEBUG: ${1:section} ===');",
      "console.log({ ${2:variables} });",
      "console.log('=== END DEBUG ===');"
    ]
  }
}
```

---

## **⚡ CONFIGURACIÓN RÁPIDA**

### **CREAR TU PRIMER SNIPPET:**
1. **Ctrl + Shift + P**
2. **"Preferences: Configure User Snippets"**
3. **Selecciona "javascript.json"** (o tu lenguaje)
4. **Pega alguno de los ejemplos anteriores**

### **EJEMPLO DE USO:**
- Escribe `cl` + Tab → `console.log('variable:', variable);`
- Escribe `rfc` + Tab → Componente React completo

---

## **🔍 VER TODOS LOS SNIPPETS DISPONIBLES**
```typescript
Ctrl + Shift + P           // Abrir command palette
Escribe "Insert Snippet"   // Ver todos los snippets
```