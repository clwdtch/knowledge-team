# Knowledge Team

O **Knowledge Team** é uma estrutura organizacional de agentes especializada em construir, manter, avaliar e evoluir a capacidade cognitiva de uma organização no **Paperclip**.

Em vez de misturar descoberta de conhecimento, curadoria, infraestrutura, aprendizado e avaliação em um único agente, o Knowledge Team separa essas responsabilidades em papéis claros. Isso permite uma operação mais robusta, auditável, escalável e replicável.

## Objetivo

O Knowledge Team existe para:

- estruturar a infraestrutura de conhecimento da organização
- descobrir e selecionar conhecimentos úteis para diferentes agentes
- incorporar conhecimento nas bases corretas
- manter o acervo limpo, organizado e utilizável
- governar aprendizados gerados pela operação
- garantir que agentes operacionais usem corretamente a base de conhecimento
- medir a qualidade e o impacto do sistema de knowledge

Em resumo: o Knowledge Team melhora continuamente os agentes operacionais da organização por meio de conhecimento governado. Ele **não substitui** esses agentes.

## Organização-mãe

Este repositório nasce no contexto da organização **Knowledge Force**, que atua como organização-mãe para desenvolver, testar, melhorar e depois replicar esse modelo em outras organizações.

## Liderança e papéis do time

O Knowledge Team é liderado por:

- **Chief Knowledge Officer**

E coordena os seguintes papéis:

1. **Knowledge Infra**
2. **Knowledge Architect**
3. **Knowledge Librarian**
4. **Knowledge Discovery**
5. **Knowledge Curator**
6. **Knowledge Finder**
7. **Learning Manager**
8. **Knowledge Enablement**
9. **Knowledge Evaluator**

## Papel de cada agente

### Chief Knowledge Officer
Lidera o Knowledge Team, define a estratégia de conhecimento e contrata os demais agentes do time.

### Knowledge Infra
Garante que a infraestrutura técnica necessária para o time operar esteja instalada, configurada e saudável.

### Knowledge Architect
Define a arquitetura, a taxonomia e a estrutura geral da base de conhecimento.

### Knowledge Librarian
Mantém o acervo organizado, limpo, atualizado e livre de redundâncias.

### Knowledge Discovery
Pesquisa continuamente referências, livros, artigos, frameworks e boas práticas relevantes por função.

### Knowledge Curator
Seleciona, entre os conhecimentos descobertos, o que faz sentido para cada tipo de agente da organização.

### Knowledge Finder
Localiza, coleta e incorpora os materiais aprovados na base de conhecimento correta.

### Learning Manager
Governa os aprendizados gerados pelos agentes operacionais, separando ruído, memória revisável e instrução permanente.

### Knowledge Enablement
Garante que os agentes operacionais consultem a base de conhecimento e encaminhem aprendizados corretamente.

### Knowledge Evaluator
Mede a qualidade, o impacto e as lacunas do sistema de knowledge.

## Princípios do sistema

### 1. Separação de responsabilidades
Cada papel tem uma função clara. Descobrir, selecionar, ingerir, organizar, aprender, habilitar e avaliar são atividades diferentes e não devem ser confundidas.

### 2. Governança de aprendizado
Nem todo aprendizado observado pelos agentes deve virar instrução permanente. O sistema separa aprendizado bruto de aprendizado validado.

### 3. Conhecimento como infraestrutura
A base de conhecimento não é só conteúdo. Ela depende de arquitetura, manutenção, higiene, avaliação e adoção operacional.

### 4. Evolução contínua
O sistema deve aprender com a operação, melhorar com o tempo e manter rastreabilidade sobre o que mudou e por quê.

### 5. Replicabilidade
O Knowledge Team foi pensado para ser instalado em outras organizações, preservando consistência e qualidade.

## Fluxo geral de funcionamento

1. **Knowledge Infra** garante que a infraestrutura esteja pronta
2. **Knowledge Architect** define a estrutura da base
3. **Knowledge Librarian** mantém o acervo saudável
4. **Knowledge Discovery** descobre fontes e referências
5. **Knowledge Curator** seleciona o que faz sentido
6. **Knowledge Finder** encontra e incorpora os materiais aprovados
7. **Learning Manager** governa aprendizados gerados pela operação
8. **Knowledge Enablement** garante que os agentes usem corretamente o sistema
9. **Knowledge Evaluator** mede impacto, qualidade e lacunas
10. **Chief Knowledge Officer** supervisiona a coerência estratégica do todo

## Relação com agentes operacionais

Os agentes do Knowledge Team **não substituem os agentes operacionais** da organização.

Os agentes operacionais continuam sendo os responsáveis por executar o trabalho-fim da empresa: marketing, finanças, vendas, jurídico, produto, operações, suporte e outras áreas.

O papel do Knowledge Team é elevar a qualidade desses agentes, oferecendo:

- melhor base de conhecimento
- melhor governança de aprendizado
- melhor estrutura de consulta
- melhor manutenção do acervo
- melhor avaliação do sistema

## Papel do AnythingLLM e do Paperclip

### AnythingLLM
O **AnythingLLM** funciona como base consultiva de conhecimento de domínio: livros, artigos, playbooks, documentos e referências que os agentes podem consultar.

### Paperclip
O **Paperclip** funciona como ambiente operacional e organizacional do sistema, incluindo a gestão prática dos agentes e dos fluxos do time.

No cenário atual, existe um plugin local do Paperclip que adiciona um menu **"Knowledge"** e abre o **AnythingLLM**. Esse plugin já existe no ambiente local de referência, mas **ainda não está publicado em repositório oficial**. Portanto, ele ainda não pode ser tratado nesta documentação como dependência pública replicável.

### Learning Manager
O **Learning Manager** governa os aprendizados produzidos pela operação e decide o que deve ser descartado, consolidado ou promovido.

## Repositório como fonte de verdade

Este repositório deve ser usado como fonte de verdade para:

- instruções dos agentes do Knowledge Team
- templates de contratação
- estrutura organizacional do time
- documentação da arquitetura
- evolução futura do sistema

Ao contratar ou atualizar agentes do Knowledge Team, priorize sempre o conteúdo deste repositório.

## Implementação rápida

Se o objetivo é colocar o sistema de pé com o menor atrito possível, use esta sequência:

1. contrate o **Chief Knowledge Officer**
2. mande o CKO consultar este repositório
3. contrate o **Knowledge Infra** para validar a stack mínima
4. contrate os agentes centrais de estruturação
5. ative o **Learning Manager**
6. valide adoção com **Knowledge Enablement**
7. meça com **Knowledge Evaluator**

Documentos operacionais para isso:

- `docs/quickstart.md` — passo a passo curto e executável
- `IMPLEMENTATION.md` — checklist operacional de implantação real
- `docs/bootstrap.md` — ordem e lógica do bootstrap
- `docs/paperclip-knowledge-plugin.md` — status atual da dependência do plugin Knowledge e critérios para replicação

## Estrutura do repositório

```text
knowledge-team/
├─ README.md
├─ IMPLEMENTATION.md
├─ agents/
│  ├─ chief-knowledge-officer.md
│  ├─ knowledge-infra.md
│  ├─ knowledge-architect.md
│  ├─ knowledge-librarian.md
│  ├─ knowledge-discovery.md
│  ├─ knowledge-curator.md
│  ├─ knowledge-finder.md
│  ├─ learning-manager.md
│  ├─ knowledge-enablement.md
│  └─ knowledge-evaluator.md
├─ templates/
│  ├─ hire-knowledge-infra.md
│  ├─ hire-knowledge-architect.md
│  ├─ hire-knowledge-librarian.md
│  ├─ hire-knowledge-discovery.md
│  ├─ hire-knowledge-curator.md
│  ├─ hire-knowledge-finder.md
│  ├─ hire-learning-manager.md
│  ├─ hire-knowledge-enablement.md
│  └─ hire-knowledge-evaluator.md
└─ docs/
   ├─ architecture.md
   ├─ bootstrap.md
   ├─ operating-model.md
   ├─ paperclip-knowledge-plugin.md
   └─ quickstart.md
```
