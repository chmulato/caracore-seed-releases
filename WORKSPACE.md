# Workspace local — CaraCore Seed (releases)

Este documento descreve o **workspace local** do repositório público de delivery do CaraCore Seed e o fluxo de **releases** e **novas features**.

---

## Repositório remoto (delivery)

- **URL:** https://github.com/chmulato/caracore-seed-releases  
- **Clone (HTTPS):** `https://github.com/chmulato/caracore-seed-releases.git`  
- **Nome do repositório:** `caracore-seed-releases`

## Workspace local

- **Caminho local:** `D:\dev\caracore-seed-releases`  
- Uso: trabalhar com novas features, documentação de delivery, conteúdo público e tags de release sem alterar o repositório principal (**caracore-seed**).

### Configurar o remote (primeira vez)

Se você criou ou clonou a pasta localmente e ainda não vinculou ao GitHub:

```bash
git remote add origin https://github.com/chmulato/caracore-seed-releases.git
git branch -M main
git push -u origin main
```

Se o remote já existir com outro nome ou URL:

```bash
git remote set-url origin https://github.com/chmulato/caracore-seed-releases.git
```

---

## Estrutura do workspace

| Pasta/arquivo | Uso |
|---------------|-----|
| **README.md** | Apresentação do projeto, foco offline/Windows e links. |
| **WORKSPACE.md** | Este arquivo — workspace local e repositório remoto. |
| **CHANGELOG.md** | Histórico de versões e mudanças de delivery. |
| **VERSION** | Número da versão atual (ex.: 1.0.0). |
| **LICENSE** | Licença do conteúdo público (se aplicável). |
| **index.html** | Portal de delivery (estilo Minerador 4.0): apresentação do CaraCore Seed, navegação e link para download. |
| **download.html** | Página de download: redireciona o cliente para [Releases → Latest](https://github.com/chmulato/caracore-seed-releases/releases/latest) para baixar **caracore-seed.exe** (versionado). |
| **.nojekyll** | Para GitHub Pages: serve os HTML sem Jekyll. |
| **docs/** (opcional) | Conteúdo estático adicional, se necessário. |

---

## Fluxo de trabalho

1. **Desenvolvimento** — Novas funcionalidades e o aplicativo desktop (Electron, SQLite) são desenvolvidos no repositório principal **caracore-seed** (D:\dev\caracore-seed).

2. **Delivery** — Quando uma release ou conteúdo público está pronto:
   - Atualize **VERSION** e **CHANGELOG.md** neste workspace.
   - Commit e push para `caracore-seed-releases`:
     ```bash
     cd D:\dev\caracore-seed-releases
     git add .
     git commit -m "chore: release 1.0.0 / documentação delivery"
     git push origin main
     ```
   - Opcionalmente crie uma **tag** (ex.: `v1.0.0`) para releases do instalador ou artefatos.

3. **Portfólio** — O site Cara Core Informática lista o CaraCore Seed como **quarto produto** e aponta para este repositório (Ver no GitHub — caracore-seed-releases).

---

## Foco do produto

- **100% offline** no Windows.  
- **Aplicativo desktop** com Electron; backend com SQLite local.  
- **Contador de Clientes** (Cara Core) e **comprador** podem usar o aplicativo local para gestão e consulta de licenças.

*Cara Core Informática.*
