# Changelog — CaraCore Seed (releases)

Repositório público de **delivery** do CaraCore Seed. Alterações notáveis deste repositório e das releases do aplicativo desktop são documentadas aqui.

**Foco:** piloto público e gratuito local sob MIT, com Electron, Java 25, Tomcat embutido e SQLite. Candidato Windows x64 0.1.3 publicado para avaliação, sem convite ou cadastro prévio e ainda sem homologação independente; Linux fica fora desta etapa. Sem checkout ou pagamento real.

---

## Candidato 0.1.3 — publicado para avaliação (2026-10-13)

- Suíte automatizada aprovada: Maven 914 testes; launcher 2/2; Electron 6/6; validação do pacote aprovada.
- Instalador Windows x64 unsigned publicado em `v0.1.3`: [release](https://github.com/chmulato/caracore-seed-releases/releases/tag/v0.1.3). SHA-256 `5adf48b1b8b14d79ff55fc7aecc1f38f7d4ee221848b68af3bae58e5a83626e8`.
- Piloto público e aberto, no mesmo princípio de distribuição do PDV Rust; sem processo de convite. Isso não transfere limites, funcionalidades ou regras comerciais entre produtos.
- Disponibilizado para avaliação antes da homologação independente; instalação/uso em perfil limpo e regressões manuais continuam pendentes. Não declarar homologado nem pronto para produção.
- Primeiro acesso: `admin` / `admin`, troca obrigatória por senha de exatamente 8 caracteres com confirmação e chave de recuperação.
- Seed opera localmente com SQLite e servidor em `127.0.0.1`; não oferece monitoramento remoto de heartbeats.
- Linux permanece fora até build e smoke em runner Linux nativo. Não orientar a desativar proteções do Windows.

## 0.1.0 — registro histórico do piloto

### Alterações

- A edição piloto é gratuita, sob MIT, e não exige ativação do próprio Seed.
- O registro de `0.1.0` foi mantido como histórico; esta versão não é o candidato atual e não deve ser tratada como pacote disponível.
- O candidato atual para avaliação é o `0.1.3` descrito acima. A senha inicial vigente é `admin` e a troca obrigatória pede senha de exatamente 8 caracteres, confirmação e chave de recuperação.
- Não há checkout nem processamento real de pagamentos; o gateway permanece simulado.

### Estado

- Não oferecer `0.1.0` para download nem inferir homologação a partir deste registro.
- Consultar a seção do candidato `0.1.3`; release pública não equivale a homologação ou prontidão para produção.

---

## [1.0.0] — 2026-02-05

> **Obsoleta, sem suporte:** esta versão pertence à linha anterior do projeto e não é o candidato atual para avaliação. Consulte a versão 0.1.3 acima.

### Adicionado

- Estrutura inicial do repositório público **[caracore-seed-releases](https://github.com/chmulato/caracore-seed-releases)**.
- README com foco em aplicativo 100% offline no Windows e gestão de licenças do ecossistema CaraCore.
- WORKSPACE.md com workspace local `D:\dev\caracore-seed-releases` e repositório remoto para delivery.
- CaraCore Seed definido como **quarto produto** no portfólio da Cara Core Informática; link para este repositório.

### Notas

- O código-fonte e o desenvolvimento do CaraCore Seed permanecem no repositório principal (caracore-seed). Este repositório contém a vitrine pública e a gestão de releases/delivery.

---

[1.0.0]: https://github.com/chmulato/caracore-seed-releases/releases/tag/v1.0.0
