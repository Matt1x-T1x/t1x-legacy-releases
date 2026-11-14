# T1x Legacy

> **Ecossistema:** Matt1x / T1x  
> **Versão Atual:** `v0.1.0 - Seed`  
> **Arquitetura:** Local-First, Open-Format (50+ Years Durability) & Web-Ready

**T1x Legacy** é um Sistema Operacional de Origem, Consciência, Ciência e Legado — uma ponte viva entre o passado profundo da humanidade, a história de cada família, o rigor da ciência moderna e o futuro que estamos construindo.

---

## Manifesto & Pilares

1. **Longevidade Geracional (50+ anos):** Todos os registros são armazenados em arquivos **Markdown (`.md`)** com metadados em **YAML Frontmatter**, legíveis por humanos e máquinas independentemente de empresas ou plataformas.
2. **Privacidade Total (Local-First / BYOV):** O código funciona apenas como motor visual e estrutural. Seus dados íntimos (`/vault/01-roots` e `/vault/03-horizon`) são protegidos pelo `.gitignore` e nunca entram no histórico do repositório.
3. **Arquitetura Híbrida (`VaultStorageProvider`):** Lê diretamente do sistema de arquivos local hoje e está preparado para operar no navegador (File System Access API / IndexedDB) em futuros deploys web.

---

## A Árvore Viva (4 Camadas)

| Camada | Diretório | Significado | Cor Telemetria |
| :--- | :--- | :--- | :--- |
| **0. Chronos** | `/vault/00-chronos` | Raízes Profundas — Engenhosidade da humanidade | `#FACC15` (Astro) |
| **1. Roots** | `/vault/01-roots` | Raízes Próximas — Linhagem e memória familiar | `#10B981` (Life) |
| **2. Codex** | `/vault/02-codex` | O Tronco — Sabedoria ancestral + Ciência moderna | `#FF6A1A` (Fire) |
| **3. Horizon** | `/vault/03-horizon` | A Copa e os Frutos — Diário e Cápsula do Tempo | `#F4F4F6` / `#FF6A1A` |

---

## Como Executar Localmente

```bash
# 1. Instalar dependências
npm install

# 2. Iniciar servidor de desenvolvimento
npm run dev

# 3. Build de produção
npm run build
```

Acesse `http://localhost:3000` para abrir o **Hub Central da Árvore Viva**.
