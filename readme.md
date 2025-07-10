# Configuração Personalizada para VS Code

Este arquivo JSON contém uma configuração personalizada para deixar seu Visual Studio Code mais limpo, bonito e funcional. Ele ajusta temas, fonte, minimapa, barra de status, entre outros detalhes.

## ✅ Pré-requisitos

- [Visual Studio Code](https://code.visualstudio.com/) instalado
- Extensões recomendadas (instale pela aba de extensões do VScode):

  - **Rosé Pine Theme**
  - **Symbols Icon Theme**
  - **JetBrains Mono Font** — instale manualmente ou via [JetBrains Mono](https://www.jetbrains.com/lp/mono/)
  - (Opcional) Outras extensões mencionadas: `glassit`, `todo-tree`, `vscord`.

## ⚙️ Como aplicar as configurações

1. Abra o **VS Code**.
2. Pressione `Ctrl + Shift + P` para abrir a **paleta de comandos**.
3. Digite `Preferences: Open User Settings (JSON)` e selecione.
4. Copie e cole o conteúdo abaixo no arquivo que será aberto:

```json
{
    "workbench.colorTheme": "Rosé Pine",
    "workbench.iconTheme": "symbols",
    "editor.fontFamily": "JetBrains Mono",
    "editor.fontSize": 16,
    "editor.lineHeight": 1.8,
    "editor.renderLineHighlight": "gutter",
    "editor.minimap.enabled": false,
    "editor.semanticHighlighting.enabled": false,
    "editor.scrollbar.horizontal": "hidden",
    "editor.cursorBlinking": "phase",
    "editor.overviewRulerBorder": false,
    "editor.renderWhitespace": "none",
    "files.autoSave": "afterDelay",
    "files.exclude": {
        "**/__pycache__": true,
        "**/.DS_Store": true,
        "**/.env": true
    },
    "explorer.compactFolders": false,
    "explorer.confirmDelete": false,
    "explorer.confirmDragAndDrop": false,
    "workbench.startupEditor": "newUntitledFile",
    "workbench.editor.labelFormat": "short",
    "workbench.editor.showTabs": "none",
    "workbench.editor.editorActionsLocation": "hidden",
    "workbench.editor.empty.hint": "hidden",
    "workbench.statusBar.visible": false,
    "workbench.layoutControl.enabled": false,
    "window.commandCenter": false,
    "window.menuBarVisibility": "toggle",
    "window.titleBarStyle": "custom",
    "window.title": "${dirty}${activeEditorShort}",
    "git.enabled": false,
    "breadcrumbs.enabled": false,
    "security.workspace.trust.untrustedFiles": "open",
    "python.createEnvironment.trigger": "off",
    "glassit.alpha": 255,
    "todo-tree.highlights.defaultHighlight": {},
    "vscord.app.name": "Code",
    "vsicons.dontShowNewVersionMessage": true,
    "explorer.fileNesting.patterns": {
        "*.ts": "${capture}.js",
        "*.js": "${capture}.js.map, ${capture}.min.js, ${capture}.d.ts",
        "*.jsx": "${capture}.js",
        "*.tsx": "${capture}.ts",
        "tsconfig.json": "tsconfig.*.json",
        "package.json": "package-lock.json, yarn.lock, pnpm-lock.yaml, bun.lockb, bun.lock",
        "Cargo.toml": "Cargo.lock",
        "*.sqlite": "${capture}.${extname}-*",
        "*.db": "${capture}.${extname}-*",
        "*.sqlite3": "${capture}.${extname}-*",
        "*.db3": "${capture}.${extname}-*",
        "*.sdb": "${capture}.${extname}-*",
        "*.s3db": "${capture}.${extname}-*"
    },
    "workbench.activityBar.location": "hidden",
    "editor.guides.indentation": true,
    "editor.cursorSmoothCaretAnimation": "on",
    "editor.smoothScrolling": true,
    "terminal.integrated.smoothScrolling": true,
    "terminal.integrated.fontSize": 14
}
```