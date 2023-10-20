## Configuração de Chave SSH e Repositório Git no Termux

### Etapa 1: Verificar a existência de uma chave SSH

Para verificar se você já possui uma chave SSH, execute o seguinte comando no Termux:

```shell
ls ~/.ssh
```

### Etapa 2: Configurar o repositório Git para usar SSH

Altere a URL remota do seu repositório Git para usar SSH com o seguinte comando, substituindo `seu_nome_de_usuário` e `seu_projeto` pelos valores reais do seu repositório:

```shell
git remote set-url origin git@github.com:seu_nome_de_usuário/seu_projeto.git
```

### Etapa 3: Gerar uma chave SSH (caso não tenha uma)

Se você ainda não possui uma chave SSH, siga estas etapas para gerar uma. Substitua `seu_email@example.com` pelo seu endereço de e-mail real:

```shell
ssh-keygen -t ed25519 -C "seu_email@example.com"
```

### Etapa 4: Copiar a chave pública SSH

Use o seguinte comando para exibir a chave pública SSH:

```shell
cat ~/.ssh/id_ed25519.pub
```

Siga estas etapas para configurar com sucesso chaves SSH e repositórios Git no Termux. Certifique-se de substituir as informações entre colchetes pelas informações reais do seu projeto e e-mail.
