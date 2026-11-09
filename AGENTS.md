# Guia de Operação 100% na Nuvem — `alexa-chefao`
> **Para Agentes de IA (Antigravity Cloud, OpenAI Codex Cloud, xAI Grokbot, Claude Code & GitHub Codespaces)**

Este arquivo (`.agents/CLOUD_GUIDE.md`) ensina qualquer agente autônomo ou desenvolvedor na nuvem a operar, compilar, testar e localizar arquivos de suporte deste projeto **sem depender do computador local**.

---

## 1. Identidade e Arquitetura
- **Repositório GitHub:** `https://github.com/pngjaico/alexa-chefao`
- **Stack Principal:** Skill / Integração Alexa (alexa-chefao).
- **Branch Padrão:** `main`

### Mapa de Branches & Variantes Disponíveis
- **`main`** (Branch Padrão)

> **Atenção Agentes:** Se existir a branch `sync-pc-2026-11-08` ou branches de variantes listadas acima, verifique-as com `git branch -a` / `git checkout <branch>` caso procure experimentos específicos ou o último snapshot incremental do PC.

---

## 2. Referenciação Cruzada no Google Drive (`pngjaico@gmail.com`)

Todo material que **não é código** (datasets, PDFs, pacotes mínimos de assets, dumps e backups) e todos os **segredos/credenciais** vivem no Google Drive estruturado:

1. **Pasta do Projeto no Drive (`Projetos/alexa-chefao/`):**
   - **Link Direto:** https://drive.google.com/drive/folders/11nh7YZ7hJ0xYaKB18po5QJYuKgWrcM3R
   - **Subpastas padrão:** `docs/`, `dados/`, `assets/`, `backups/`
2. **Pasta Restrita de Segredos e Dados Sensíveis (`Projetos/_Restrito/alexa-chefao/`):**
   - **Link Direto:** https://drive.google.com/drive/folders/1nlGk3DLdEepOVz4x3eKRR_cPDpFhv-AW
   - **Itens Restritos / Segredos Mapeados:**
  - Nenhum segredo obrigatório registrado neste snapshot (consulte `_Restrito` geral se necessário).
3. **Pasta Raiz `Projetos/` no Drive:**
   - **Link Direto:** https://drive.google.com/drive/folders/11nh7YZ7hJ0xYaKB18po5QJYuKgWrcM3R

---

## 3. Comandos de Execução no Ambiente Cloud (Codespaces / Antigravity / Codex / Grokbot)

- **Instalação de dependências:**
  ```bash
  Consulte README.md
  ```
- **Ambiente de Desenvolvimento (Dev Server / CLI):**
  ```bash
  Consulte README.md
  ```
- **Build / Empacotamento:**
  ```bash
  N/A
  ```
- **Testes / Verificação:**
  ```bash
  N/A
  ```

---

## 4. Variáveis de Ambiente e Regras de Segurança
- **Variáveis mapeadas (`.env.example`):** Nenhuma variável obrigatória detectada (ou veja `.env.example`).
- **Regra de Ouro:** Nunca faça commit de arquivos `.env` reais, chaves `.json` de Service Accounts do Firebase/GCP, chaves `.key` ou dados identificáveis de pacientes no GitHub. Injete-os apenas como **Secrets** do ambiente cloud (GitHub Codespaces Secrets / Codex Environment Variables) buscando os valores em `Projetos/_Restrito/alexa-chefao/`.
