# Changelog — CaraCore Seed (releases)

Repositório público de **delivery** do CaraCore Seed. Alterações notáveis deste repositório e das releases do aplicativo desktop são documentadas aqui.

**Foco:** piloto gratuito local sob MIT, com Electron, Java 25, Tomcat embutido e SQLite. Candidato Windows x64 0.1.3 em homologação independente, sem download público; Linux fica fora desta etapa. Sem checkout ou pagamento real.

---

## Candidato 0.1.3 — homologação independente pendente (2026-10-13)

- Suíte automatizada aprovada: Maven 914 testes; launcher 2/2; Electron 6/6; validação do pacote aprovada.
- Candidato Windows x64 unsigned gerado localmente, mas ainda sem instalação/uso em perfil limpo e sem regressão manual completa.
- Nenhum instalador foi enviado, publicado ou disponibilizado para download. Homologação será realizada por outra IA; aguardar aceite antes de distribuir.
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
- Consultar a memória atual da oficina e a seção do candidato `0.1.3` para o gate real de distribuição.

---

## [1.0.0] — 2026-02-05

### Adicionado

- Estrutura inicial do repositório público **[caracore-seed-releases](https://github.com/chmulato/caracore-seed-releases)**.
- README com foco em aplicativo 100% offline no Windows e gestão de licenças do ecossistema CaraCore.
- WORKSPACE.md com workspace local `D:\dev\caracore-seed-releases` e repositório remoto para delivery.
- CaraCore Seed definido como **quarto produto** no portfólio da Cara Core Informática; link para este repositório.

### Notas

- O código-fonte e o desenvolvimento do CaraCore Seed permanecem no repositório principal (caracore-seed). Este repositório contém a vitrine pública e a gestão de releases/delivery.

---

[1.0.0]: https://github.com/chmulato/caracore-seed-releases/releases/tag/v1.0.0
