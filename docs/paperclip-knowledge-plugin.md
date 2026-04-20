# Plugin `Knowledge` do Paperclip

Status operacional da dependência que conecta o menu `Knowledge` do Paperclip ao AnythingLLM.

## Estado atual

No ambiente de referência atual:

- o plugin existe localmente no Paperclip
- ele cria um menu **`Knowledge`**
- ao acionar esse menu, o fluxo abre o **AnythingLLM**
- esse plugin **ainda não está publicado em repositório oficial**

Conclusão: a integração existe e pode ser validada no ambiente local atual, mas **ainda não é uma dependência replicável por documentação pública de instalação**.

## Como tratar essa dependência nesta documentação

Até a publicação oficial do plugin, trate o item assim:

- **dependência existente localmente** no ambiente de referência
- **pré-requisito pendente para replicação** em outras organizações
- **placeholder operacional** para bootstrap fora do ambiente que já possui o plugin

Ou seja: a documentação pode mandar validar o plugin no ambiente atual, mas não pode afirmar que basta instalar um pacote público já disponível.

## O que o Knowledge Infra deve verificar hoje

1. se o menu `Knowledge` aparece no Paperclip
2. se o clique no menu abre o AnythingLLM esperado
3. qual é a URL do AnythingLLM usada no ambiente
4. se a navegação funciona sem erro de permissão, rota ou conectividade
5. se a dependência está registrada como **local-only**, **publicada** ou **bloqueada**

## O que precisa existir para isso ficar replicável

Para a implantação ficar replicável em outra organização, ainda falta documentar e publicar pelo menos:

- repositório oficial do plugin
- instrução oficial de instalação
- versão mínima compatível do Paperclip
- forma de configurar a URL do AnythingLLM
- forma de validar que o menu `Knowledge` apareceu
- forma de validar que o menu abre o destino correto
- política de credenciais, permissões e dependências relacionadas

Sem isso, a implantação completa continua com dependência pendente.

## Checklist pós-publicação

Quando o plugin for publicado, atualizar este repositório com:

- URL do repositório oficial
- nome exato do plugin/pacote
- passo a passo de instalação
- passo a passo de configuração da URL do AnythingLLM
- evidência esperada de validação do menu `Knowledge`
- limitações conhecidas e troubleshooting mínimo

## Formulação recomendada

Use formulações como:

- "existe um plugin local `Knowledge` no ambiente atual"
- "a publicação oficial do plugin é pré-requisito para replicação"
- "enquanto não houver publicação oficial, esta dependência deve ser tratada como pendência operacional"

Evite formulações como:

- "instale o plugin"
- "adicione a dependência"
- "siga o repositório do plugin"

Essas frases só passam a ser corretas depois da publicação oficial.
