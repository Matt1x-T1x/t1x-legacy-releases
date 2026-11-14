# Changelog — T1x Legacy

Todas as mudanças notáveis deste projeto são documentadas neste arquivo seguindo [Semantic Versioning](https://semver.org/).

## [1.1.2] - 2026-11-14 — `Desktop`

### Corrigido & Aprimorado
- **Servidor Standalone no Instalador Windows:** Adicionado hook `scripts/after-pack.mjs` garantindo inclusão de `.next/standalone/node_modules` em `resources/standalone/node_modules` (resolvendo travamento na Splash Screen).
- **Tratamento de Erro na Inicialização:** `electron/main.ts` fecha a Splash Screen e exibe diálogo claro caso o servidor local falhe ao iniciar.
- **Identidade Matt1x Terminal Pop:** Aplicados tokens `--m1x-*`, fontes `IBM Plex Mono` e `IBM Plex Sans`, assinatura `matt1x / T1x Legacy_` e barra sólida `#FF6A1A` na Splash Screen.
- **UX de Primeiro Acesso:** Adicionado guia rápido no Hub Central e botões diretos `"Explorar <Módulo> →"` em cada camada da Árvore Viva.

## [1.1.1] - 2026-11-14 — `Desktop`

### Corrigido
- **Dependência `electron-updater` em produção:** Movido `electron-updater` de `devDependencies` para `dependencies` no `package.json` para inclusão correta no `app.asar` do instalador Windows.

## [1.1.0] - 2026-11-14 — `Desktop`

### Adicionado
- **Empacotamento Windows Nativo (Electron + NSIS):** Instalador `x64` com Next.js Standalone embutido e janela nativa *Telemetria Ancestral* (`#111014`).
- **Isolamento do Vault no SO (`T1X_VAULT_PATH`):** Cofre do usuário isolado em `Documentos/T1x-Legacy/vault`, preservando dados pessoais entre atualizações.
- **Auto-Updater Integrado:** Conexão IPC segura com `Matt1x-T1x/t1x-legacy-releases` para verificar, baixar e instalar atualizações dentro do próprio app.
- **Ícone Oficial & Splash Screen:** Emblema vetorial Astrolábio + Árvore Viva (`icon.svg` / `icon.png` / `icon.ico`) e tela de abertura animada *Telemetria Ancestral*.

## [1.0.0] - 2026-11-14 — `Legacy`

### Adicionado
- **T1x Horizon (`v1.0.0`):** Diário de princípios e **Cápsula do Tempo** com selo temporal (`unlockDate`/`unlockYear`), dedicatória e contagem regressiva em estilo telemetria.
- **Paleta de Comando Global (`Ctrl+K`):** Busca instantânea entre pessoas, eras, conceitos, cápsulas e tags em todas as 4 camadas.
- **Ponte IA Local (`src/lib/ollama.ts`):** Integração opcional com Ollama local (fallback silencioso offline) para sugestões de entrevista no *Roots* e conexões *Horizon ↔ Codex*.
- **API Local (`/api/vault` e `/api/ai/suggest`):** Criação visual de registros em Markdown + YAML diretamente no `/vault` via `LocalFsVaultProvider`.
- **Canal Público de Releases:** Atualização do `updater.ts` para consultar o repositório público `t1x-legacy-releases`.

## [0.4.0] - 2026-11-14 — `Codex`

### Adicionado
- **Visão de Lentes Duplas:** Exibição lado a lado da *Lente Ancestral*, *Lente Científica* e *Protocolo Prático*.
- **Links Bidirecionais (`[[conceito]]`):** Suporte no `vault-parser.ts` + grafo visual de conexões conceituais e 6 verbetes completos.

## [0.3.0] - 2026-11-14 — `Chronos`

### Adicionado
- **Linha do Tempo por Eras:** Filtro cronológico da Pré-História à Era Digital com 6 marcos históricos e cards de engenharia.
- **2 Simuladores Interativos (SVG):** Astrolábio Planisférico (latitude, declinação, ângulo horário) e Engenhosidade Mecânica (Alavanca & Clepsidra).

## [0.2.0] - 2026-11-14 — `Roots`

### Adicionado
- **Grafo Genealógico Interativo:** Visualização com zoom, pan, destaque de linhagens e árvore exemplar de 3 gerações (`exemplo-bisavo`, `exemplo-avo`, `exemplo-mae`).
- **Dossiê Familiar & Cruzamento Histórico:** Receitas, player de áudio, galeria de fotos e marcos contemporâneos do `Chronos`.

## [0.1.0] - 2026-11-14 — `Seed`

### Adicionado
- Estrutura inicial Local-First, `.gitignore` blindado, `VaultStorageProvider`, motor Markdown + YAML e Hub Central *Telemetria Ancestral*.
