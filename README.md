# CaraCore Seed — piloto

O **CaraCore Seed** é um piloto local para cadastrar clientes e administrar licenças de software. A edição piloto é gratuita, está licenciada sob MIT e não exige licença para executar o próprio Seed. Não há checkout nem processamento real de pagamentos.

## Estado da distribuição

- O portal apresenta o produto e suas instruções.
- O candidato Windows x64 `0.1.3` está publicado na release para avaliação. Passou nos testes automatizados, mas a homologação independente e a instalação/uso em perfil limpo estão pendentes; não o declare homologado nem pronto para produção.
- O `0.1.3` é a versão piloto pública para avaliação; sua publicação não significa homologação nem prontidão para produção.
- O piloto é aberto, sem convite ou cadastro prévio; esse modelo de distribuição segue a ideia do piloto público do PDV Rust, sem importar limites ou regras comerciais daquele produto.
- Linux fica fora desta entrega até build e smoke em runner Linux nativo.
- Os instaladores desta fase serão unsigned; nunca orientar a desativar SmartScreen, Defender ou outras proteções.
- O código-fonte está licenciado sob MIT no repositório de desenvolvimento, mas esse repositório ainda não teve sua disponibilidade pública confirmada. Não trate o piloto como publicamente acessível ao código até essa publicação.
- O Seed é local: SQLite no perfil do usuário, servidor em `127.0.0.1`, sem monitoramento remoto de heartbeats e sem checkout/pagamento real.
- Release `v0.1.3`: [baixar instalador Windows x64](https://github.com/chmulato/caracore-seed-releases/releases/download/v0.1.3/caracore-seed-0.1.3-windows-x64.exe). SHA-256: `5adf48b1b8b14d79ff55fc7aecc1f38f7d4ee221848b68af3bae58e5a83626e8`. Instalador unsigned; nunca desative as proteções do Windows.

## O aplicativo

- Aplicação desktop Electron com backend Java 25 e Tomcat embutido.
- SQLite local no perfil do usuário; API do servidor limitada a `127.0.0.1`.
- Cadastro de clientes, administração/validação de licenças, auditoria, alertas e heartbeats.
- Primeiro acesso: `admin` / `admin`; a troca é obrigatória por senha nova de exatamente 8 caracteres, com confirmação. Copiar a chave de recuperação exibida no primeiro acesso e guardá-la fora do computador. Recuperar pela chave; nunca remover manualmente o arquivo de credenciais nem o banco.
- `StubPaymentGateway` é apenas uma simulação para testes e desenvolvimento.

## Repositórios e links

- **Vitrine:** [seed.caracore.com.br](https://seed.caracore.com.br/)
- **Downloads:** [página de download](https://seed.caracore.com.br/download.html)
- **Releases desta loja:** [GitHub Releases](https://github.com/chmulato/caracore-seed-releases/releases)
- **Matriz:** [portfolio.html#caracore-seed](https://www.caracore.com.br/portfolio.html#caracore-seed)
- **Texto da licença MIT do binário:** [LICENSE](https://github.com/chmulato/caracore-seed-releases/blob/master/LICENSE)
- **Estado do código-fonte:** não está publicado neste repositório; não há data definida para publicação.

Este repositório mantém a vitrine e poderá receber artefatos somente após os gates de homologação. Não contém a oficina nem os binários públicos da aplicação neste momento.
