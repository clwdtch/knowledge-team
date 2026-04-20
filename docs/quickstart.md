# Quickstart do Knowledge Team

Guia curto para colocar o Knowledge Team de pé sem ficar interpretando o repositório inteiro.

## Objetivo

Ao final deste quickstart, você deve ter:

- um **Chief Knowledge Officer (CKO)** contratado
- o repositório como fonte de verdade consultada
- os agentes centrais contratados na ordem certa
- a infraestrutura mínima validada
- o fluxo de consulta + aprendizado funcionando
- uma validação inicial de adoção concluída

---

## Pré-requisitos

Antes de começar, confirme:

- organização já existente no **Paperclip**
- acesso operacional para contratar agentes
- **AnythingLLM** disponível ou em fase final de instalação
- entendimento explícito de que o plugin `Knowledge` do **Paperclip** existe localmente no ambiente de referência, mas ainda não foi publicado em repositório oficial
- este repositório acessível: `https://github.com/clwdtch/knowledge-team`

Se isso ainda não existir, não avance para contratação em massa. Comece pelo CKO e pelo Knowledge Infra.

### Observação crítica sobre o plugin Knowledge

Hoje existe um plugin local do Paperclip que cria o menu **"Knowledge"** e abre o **AnythingLLM**.

Esse plugin **ainda não está em repositório oficial**. Então:

- ele pode ser validado no ambiente local atual
- ele **não** pode ser tratado como dependência pública já instalável
- qualquer implantação em outra organização continua dependendo da publicação desse plugin ou de instrução equivalente oficial

Referência operacional: `docs/paperclip-knowledge-plugin.md`

---

## Fluxo mínimo recomendado

## Passo 1 — Contrate o Chief Knowledge Officer

O CKO é o agente de entrada.

Ele deve receber como instrução inicial que:

- lidera o Knowledge Team
- usa este repositório como fonte de verdade
- contrata os demais agentes
- segue a ordem de bootstrap do repositório
- reporta bloqueios de implantação

Referência principal:

- `agents/chief-knowledge-officer.md`

---

## Passo 2 — Mande o CKO consultar o repositório

Peça explicitamente para o CKO ler pelo menos:

- `README.md`
- `docs/bootstrap.md`
- `docs/architecture.md`
- `docs/operating-model.md`

Objetivo desta etapa:

- alinhar a ordem de implantação
- alinhar os papéis
- alinhar o uso de AnythingLLM, Paperclip e Learning Manager

---

## Passo 3 — Contrate o Knowledge Infra primeiro

O primeiro agente contratado pelo CKO deve ser o **Knowledge Infra**.

Template de apoio:

- `templates/hire-knowledge-infra.md`

O que ele precisa validar na prática:

- se o **AnythingLLM** está instalado e acessível
- se o plugin local `Knowledge` do **Paperclip** está operacional no ambiente atual
- qual URL do **AnythingLLM** o plugin abre no ambiente atual
- se existe conectividade entre os componentes usados no fluxo real
- se há permissões, credenciais e dependências suficientes para operar

Saída mínima esperada do Knowledge Infra:

- status da stack: ok / bloqueada / parcial
- lista objetiva de bloqueios
- confirmação do ambiente mínimo utilizável
- classificação do plugin como: dependência local existente / dependência replicável publicada / bloqueio aberto

---

## Passo 4 — Contrate o núcleo de estruturação

Com a infra minimamente validada, o CKO deve contratar nesta ordem:

1. **Knowledge Architect**
2. **Knowledge Librarian**
3. **Knowledge Discovery**
4. **Knowledge Curator**
5. **Knowledge Finder**

Templates de apoio:

- `templates/hire-knowledge-architect.md`
- `templates/hire-knowledge-librarian.md`
- `templates/hire-knowledge-discovery.md`
- `templates/hire-knowledge-curator.md`
- `templates/hire-knowledge-finder.md`

Objetivo operacional desse bloco:

- definir a estrutura da base
- organizar o acervo inicial
- levantar fontes prioritárias
- selecionar o que realmente entra
- incorporar material útil na base correta

---

## Passo 5 — Contrate o Learning Manager

Template de apoio:

- `templates/hire-learning-manager.md`

O Learning Manager não serve para encher a base com qualquer observação.

Ele deve operar um funil simples:

- receber aprendizados da operação
- descartar ruído
- consolidar memória revisável
- promover para instrução permanente só quando fizer sentido

Sem essa etapa, a base tende a virar acúmulo de observação solta.

---

## Passo 6 — Contrate Enablement e Evaluator

Contrate, nesta ordem:

1. **Knowledge Enablement**
2. **Knowledge Evaluator**

Templates de apoio:

- `templates/hire-knowledge-enablement.md`
- `templates/hire-knowledge-evaluator.md`

O que cada um fecha no uso real:

- **Knowledge Enablement**: garante que os agentes operacionais consultem a base e enviem aprendizados corretamente
- **Knowledge Evaluator**: mede adoção, utilidade, lacunas e gargalos

---

## Passo 7 — Valide o bootstrap

Considere o bootstrap minimamente validado somente se você conseguir responder “sim” para tudo abaixo:

- o CKO está ativo e coordenando o time?
- o Knowledge Infra confirmou ambiente mínimo utilizável?
- o AnythingLLM está acessível para consulta?
- os agentes centrais já foram contratados?
- o Knowledge Architect definiu uma estrutura inicial?
- o Knowledge Finder já incorporou ao menos materiais aprovados?
- o Learning Manager já recebeu aprendizados de teste?
- o Knowledge Enablement já auditou ao menos 1 agente operacional?
- o Knowledge Evaluator já produziu um diagnóstico inicial?

Se a resposta for “não” para vários itens, o sistema ainda não está pronto para operação normal.

---

## Papel de cada peça no uso real

### AnythingLLM

Use como camada de **consulta de conhecimento**.

Serve para:

- livros
- artigos
- playbooks
- documentos
- referências por função

Não serve como substituto da governança do time.

### Paperclip

Use como camada **operacional e organizacional**.

É onde:

- os agentes existem
- os papéis são definidos
- a coordenação acontece
- a execução prática do time é gerida

### Learning Manager

Use como camada de **governança do aprendizado gerado pela operação**.

Ele separa:

- ruído
- memória revisável
- instrução permanente

---

## Primeira checagem de adoção

Depois do bootstrap, selecione 1 ou 2 agentes operacionais reais da organização e valide:

- eles consultam a base antes de responder temas relevantes?
- eles sabem quando acionar AnythingLLM?
- eles sabem para onde mandar aprendizados úteis?
- o Learning Manager recebeu esses aprendizados?
- houve retorno útil ou ajuste de instrução?

Se isso não acontecer no piloto, o problema normalmente não é “falta de mais conteúdo”. É falta de enablement, protocolo ou governança.

---

## Sequência curta, em uma linha

Se quiser resumir a implantação em uma sequência única:

**contrate o CKO → consulte o repo → valide infra com Knowledge Infra → contrate os agentes centrais → ative Learning Manager → valide adoção com Enablement → meça com Evaluator**
