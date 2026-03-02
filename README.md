# ⚙️ Settings

Repositorio de configuración personal de **Visual Studio Code** para mantener el mismo entorno de trabajo en cualquier equipo.

## 📁 Estructura

```text
Settings/
├── README.md
└── Visual Studio Code/
		└── settings.json
```

## 🎯 Objetivo

- Centralizar preferencias del editor.
- Mantener consistencia de estilo entre proyectos.
- Tener un backup versionado de la configuración.

## 🧩 Qué incluye la configuración

El archivo `Visual Studio Code/settings.json` contiene, entre otros:

- Editor: tabulación con tabs, tamaño 4, reglas visuales y ajuste de línea.
- Guardado/format: `formatOnSave`, limpieza de espacios finales, newline final.
- Productividad: minimapa, sticky scroll, bracket colorization, quick suggestions.
- Terminal: perfil por defecto `zsh`, scrollback alto y tema de terminal personalizado.
- Git/Copilot: `autofetch`, confirmaciones simplificadas y sugerencias activadas.
- Extensiones: ESLint, Prettier, EditorConfig, Path Intellisense, Live Server, 42header.

## 🚀 Cómo usarlo

### Opción 1: Copia directa

1. Copia el archivo a tu ruta de usuario de VS Code.
2. Reinicia VS Code.

Rutas típicas de `settings.json`:

- macOS: `~/Library/Application Support/Code/User/settings.json`
- Linux: `~/.config/Code/User/settings.json`
- Windows: `%APPDATA%\\Code\\User\\settings.json`

### Opción 2: Enlace simbólico (recomendada)

Con esto cualquier cambio en el repo se refleja al instante en VS Code.

```bash
ln -sf \
"$PWD/Visual Studio Code/settings.json" \
"$HOME/Library/Application Support/Code/User/settings.json"
```

## 🔧 Personalización rápida

- Cambia email/usuario de 42 en:
	- `42header.email`
	- `42header.username`
- Ajusta tema en `workbench.colorTheme`.
- Ajusta reglas de líneas en `editor.rulers`.
- Ajusta tamaño de fuente del terminal en `terminal.integrated.fontSize`.

## ✅ Recomendaciones

- Mantén este archivo bajo Git para conservar historial de cambios.
- Si usas varios equipos, sincroniza este repo y reutiliza el enlace simbólico.
- Si una extensión no está instalada, su clave en `settings.json` no rompe VS Code.

## 🛠️ Extensiones sugeridas

- `dbaeumer.vscode-eslint`
- `esbenp.prettier-vscode`
- `EditorConfig.EditorConfig`
- `christian-kohler.path-intellisense`
- `ritwickdey.LiveServer`
- `kube.42header`

---

💡 Tip: usa este repositorio como tu "fuente de verdad" para configuración del editor.
