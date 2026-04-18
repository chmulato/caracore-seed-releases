# CaraCore Seed — Releases e delivery

Repositório público de **delivery** do **CaraCore Seed**: gestão de licenças do ecossistema Cara Core Informática (PDV, Minerador 4.0, Reino OIDC, Hub).

**Foco:** aplicativo **100% offline** no **Windows** (Desktop com Electron e SQLite). Controle local de licenças para o Contador de Clientes e para o comprador, sem dependência de servidor na nuvem.

---

## O que é o CaraCore Seed?

O **CaraCore Seed** é o núcleo de licenciamento da suite CaraCore. Ele:

- Centraliza a gestão de licenças dos produtos: **CaraCore PDV**, **Minerador 4.0**, **Reino OIDC** e **CaraCore Hub**.
- Roda **100% offline** no Windows, com banco de dados **SQLite** local.
- É distribuído como **aplicativo desktop (EXE)** via Electron, para uso pelo Contador de Clientes (Cara Core Informática) e pelo comprador.

O desenvolvimento e o código-fonte ficam no repositório principal (**caracore-seed**). Este repositório (**caracore-seed-releases**) é o canal **público** de releases, documentação de delivery e, quando aplicável, artefatos de instalação.

---

## O que tem neste repositório?

| Onde   | O que tem |
|--------|-----------|
| **Raiz** | README, LICENSE, VERSION, CHANGELOG, WORKSPACE.md. |
| **docs/** | Portal da loja (**index.html**, **download.html**, wiki, páginas de apoio) publicado em **seed.caracore.com.br**. |
| **Releases** | Artefato versionado **caracore-seed.exe** e checksums publicados em [Releases](https://github.com/chmulato/caracore-seed-releases/releases). |

Os **clientes são direcionados à loja** (**seed.caracore.com.br**) ou ao repositório para buscar o executável da entrega (caracore-seed.exe versionado). O portal em **docs/** segue a mesma lógica de apresentação do Minerador 4.0: página inicial com apresentação do produto e navegação, e página de download com link para **Releases → Latest** quando aplicável.

---

## Espelho de delivery (mesma lógica do Reino OIDC)

| Onde | Papel |
|------|--------|
| **Domínio Cara Core Informática** | Portal completo (fonte de verdade): `D:\dev\site\cara-core\delivery\seed` |
| **Vitrine e balcão público** | Este repositório (**docs/**: index.html, download.html) e domínio **seed.caracore.com.br** — apresentação + link para Releases quando aplicável |

O **delivery/seed** no site Cara Core é o portal completo (tecnologia, portal de controle, readme). Este repo (**caracore-seed-releases**) é a **vitrine** onde o cliente encontra a apresentação e o download do EXE versionado.

---

## Links

- **Loja oficial (domínio de atendimento):** [https://seed.caracore.com.br/](https://seed.caracore.com.br/) — portal publicado a partir de **docs/** (GitHub Pages com pasta `/docs` ou espelho no site da Cara Core).
- **Portal neste repositório:** [docs/index.html](docs/index.html) — apresentação; [docs/download.html](docs/download.html) — download do **caracore-seed.exe** quando houver redirecionamento para [Releases → Latest](https://github.com/chmulato/caracore-seed-releases/releases/latest).
- **Repositório público (delivery):** [github.com/chmulato/caracore-seed-releases](https://github.com/chmulato/caracore-seed-releases)
- **Documentação do produto na loja:** [docs/wiki/projeto-seed.html](docs/wiki/projeto-seed.html) — conteúdo de apoio no mesmo domínio da loja, sem links para portfólio ou wiki em outros hosts.
- **Projeto principal (desenvolvimento):** Código-fonte e aplicação em repositório **caracore-seed** (privado ou público, conforme configuração).

Para ativar o portal no GitHub Pages: em Settings → Pages, escolha *Deploy from a branch*, branch **main** e pasta **/docs**. O arquivo **docs/.nojekyll** evita processamento Jekyll. Links de navegação do portal apontam para **seed.caracore.com.br** e para caminhos relativos dentro de **docs/** (busque por `wiki/projeto-seed.html` se precisar ajustar o destino da documentação).

---

## Produtos cujas licenças são gerenciadas

| Produto | Descrição |
|---------|-----------|
| **CaraCore PDV** | Ponto de venda; licenças e assinaturas. |
| **Minerador 4.0** (chmulato/ETE) | Simulador; chaves e Fase 2 / Ouro 4.0. |
| **Reino OIDC** | Material OAuth/OIDC; chaves e Premium (O Trono da Identidade). |
| **CaraCore Hub** | E-commerce; Centros de Distribuição e planos. |

---

*Cara Core Informática — CaraCore Seed (100% offline, Windows Desktop).*
