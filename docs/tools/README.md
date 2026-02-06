# Controle de licenças — CaraCore Seed

O **controle de licenças** do CaraCore Seed é feito na filial (este repositório), por se tratar de um negócio que pode ser vendido a um interessado. O aplicativo só funciona com uma licença válida, **presa ao sistema operacional e à placa-mãe** do computador. Respeitamos a **LGPD** em todo o processo.

## Gerador de license.key (`gerar_license_seed.py`)

Uso **interno** (administrador / Cara Core Informática). Não distribuir com o aplicativo.

### Uso

```bash
python gerar_license_seed.py <HARDWARE_ID> [VALID_UNTIL]
```

- **HARDWARE_ID:** ID de Ativação que o cliente copia do aplicativo (tela "Licença necessária"). Ex.: `A7F2C9E1B4D8`.
- **VALID_UNTIL:** Data de validade em YYYY-MM-DD (padrão: 2099-12-31).

### Exemplos

```bash
python gerar_license_seed.py A7F2C9E1B4D8
# Gera license_A7F2C9E1B4D8.key com validade 2099-12-31

python gerar_license_seed.py B3E8D1F6A2C9 2030-12-31
# Gera license com validade 2030-12-31
```

### Fluxo

1. Cliente paga R$ 29,00 (PIX) e envia comprovante + **ID de Ativação** (copiado do app) pelo [canal de feedback](https://chmulato.github.io/caracore-seed-releases/canal-feedback.html).
2. Administrador executa `python gerar_license_seed.py <ID_QUE_O_CLIENTE_ENVIOU>`.
3. Envia o conteúdo do arquivo gerado (ou o arquivo `license.key`) ao cliente.
4. Cliente coloca em `%APPDATA%\caracore-seed-desktop\license.key` (Windows) ou na pasta do executável e reinicia o app.

### Segredo

O aplicativo Electron valida a licença com o mesmo segredo usado aqui. Em produção, defina a variável de ambiente **CARA_CORE_SEED_LICENSE_SECRET** (tanto ao rodar este script quanto, se desejado, ao buildar o app) com um valor forte e único. O padrão é apenas para desenvolvimento/demonstração.

### LGPD

- O **ID de Ativação** é anônimo (não contém dados pessoais).
- A associação **ID ↔ pessoa** (nome, e-mail, telefone) fica apenas no controle administrativo (planilha, ERP), fora do software distribuído.
- Não revendemos nem compartilhamos dados.

*Cara Core Informática — Vitrine do CaraCore Seed (O Contador).*
