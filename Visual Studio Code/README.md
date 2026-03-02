# 🧩 Visual Studio Code Settings

Este directorio contiene mi configuración personal de **Visual Studio Code** para mantener el mismo entorno de trabajo entre proyectos y equipos.

## 📁 Contenido

```text
Visual Studio Code/
├── README.md
└── settings.json
```

## 🎯 Objetivo

- Tener una configuración reproducible y versionada.
- Unificar estilo de edición y comportamiento del editor.
- Mejorar productividad con reglas, formato y sugerencias.

## ⚙️ Configuración destacada

- **Editor**: tabulación con tabs (`tabSize: 4`), guías de indentación, minimapa y word wrap.
- **Guardado**: `formatOnSave`, eliminación de trailing whitespace y newline final.
- **Terminal**: perfil por defecto en macOS con `zsh`, scrollback ampliado y personalización de colores.
- **Git/Copilot**: `autofetch`, confirmaciones simplificadas y sugerencias habilitadas.
- **Calidad de código**: integración con ESLint, Prettier y EditorConfig.

## 🧰 Extensiones utilizadas

Estas extensiones aparecen configuradas en `settings.json`:

| Nombre | ID en VS Code Marketplace | Uso principal |
|---|---|---|
| GitHub Copilot | `GitHub.copilot` | Sugerencias de código asistidas por IA |
| Database Client | `cweijan.vscode-database-client2` | Exploración y consultas de bases de datos |
| ESLint | `dbaeumer.vscode-eslint` | Linting para JS/TS/Vue/HTML |
| Prettier - Code formatter | `esbenp.prettier-vscode` | Formateo automático de código |
| EditorConfig for VS Code | `EditorConfig.EditorConfig` | Respetar reglas `.editorconfig` |
| Live Server | `ritwickdey.LiveServer` | Servidor local para proyectos web |
| Path Intellisense | `christian-kohler.path-intellisense` | Autocompletado de rutas |
| 42 Header | `kube.42header` | Inserción automática del header de 42 |

## 🚀 Instalación rápida en otro equipo

1. Copia `settings.json` al path de usuario de VS Code.
2. Instala las extensiones de la tabla anterior.
3. Reinicia VS Code.

Rutas habituales de `settings.json`:

- **macOS**: `~/Library/Application Support/Code/User/settings.json`
- **Linux**: `~/.config/Code/User/settings.json`
- **Windows**: `%APPDATA%\\Code\\User\\settings.json`

## 🔧 Personalización recomendada

- Actualiza tus datos de 42:
	- `42header.email`
	- `42header.username`
- Cambia tema y colores en:
	- `workbench.colorTheme`
	- `workbench.colorCustomizations`
- Ajusta límites de línea en `editor.rulers`.

---

💡 Tip: mantener este archivo en Git facilita volver a tu entorno ideal en minutos.
