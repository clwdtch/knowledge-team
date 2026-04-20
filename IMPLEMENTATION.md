# IMPLEMENTATION.md

Checklist operacional para implementar o Knowledge Team em uma organização real.

Este documento não substitui a arquitetura nem o operating model. Ele existe para responder a uma pergunta mais simples:

**o que precisa acontecer, em ordem, para sair do zero até uma implantação utilizável?**

---

## Definição de pronto

Considere o Knowledge Team pronto para operação inicial quando:

- existe um **CKO** ativo coordenando o time
- a stack mínima foi validada pelo **Knowledge Infra**
- a base consultiva está acessível em **AnythingLLM**
- os agentes centrais foram contratados e instruídos
- existe estrutura inicial de conhecimento definida
- já ocorreu ingestão inicial de materiais aprovados
- o **Learning Manager** está recebendo aprendizados
- o **Knowledge Enablement** validou adoção mínima
- o **Knowledge Evaluator** produziu feedback inicial

Se algum desses pontos faltar, ainda existe atrito de implementação relevante.

---

## Fase 0 — Preparação

### Checklist

- [ ] Definir a organização onde o Knowledge Team será implantado
- [ ] Garantir acesso ao Paperclip para contratar e operar agentes
- [ ] Garantir acesso ao repositório `clwdtch/knowledge-team`
- [ ] Confirmar se o AnythingLLM já existe ou se ainda precisa ser instalado
- [ ] Confirmar quem resolve bloqueios de infra, credenciais e permissões
- [ ] Definir um responsável humano para destravar impedimentos do bootstrap

### Saída esperada

Existe contexto organizacional suficiente para o CKO começar sem depender de adivinhação.

---

## Fase 1 — Ponto de entrada

### Ação

Contratar o **Chief Knowledge Officer**.

### Checklist

- [ ] CKO contratado
- [ ] CKO instruído como líder do Knowledge Team
- [ ] CKO instruído a usar este repositório como fonte de verdade
- [ ] CKO instruído a seguir a ordem de bootstrap
- [ ] CKO instruído a reportar bloqueios e dependências

### Referência

- `agents/chief-knowledge-officer.md`
- `docs/bootstrap.md`

### Saída esperada

Existe um agente responsável por conduzir a implantação inteira.

---

## Fase 2 — Leitura obrigatória do repositório

### Ação

Mandar o CKO consultar o repositório antes de contratar o restante do time.

### Checklist

- [ ] CKO leu `README.md`
- [ ] CKO leu `docs/bootstrap.md`
- [ ] CKO leu `docs/architecture.md`
- [ ] CKO leu `docs/operating-model.md`
- [ ] CKO conseguiu explicar a ordem de contratação
- [ ] CKO conseguiu explicar o papel de AnythingLLM, Paperclip e Learning Manager

### Saída esperada

O CKO está alinhado com o modelo e não vai improvisar a implantação.

---

## Fase 3 — Infraestrutura mínima

### Ação

Contratar o **Knowledge Infra**.

### Checklist

- [ ] Knowledge Infra contratado
- [ ] AnythingLLM validado ou bloqueios documentados
- [ ] Paperclip/plugin/integrações validados ou bloqueios documentados
- [ ] Dependências técnicas verificadas
- [ ] Conectividade entre componentes verificada
- [ ] Credenciais e permissões mínimas verificadas
- [ ] Resultado consolidado como: pronto / parcial / bloqueado

### Referência

- `agents/knowledge-infra.md`
- `templates/hire-knowledge-infra.md`

### Saída esperada

Você sabe objetivamente se o ambiente suporta o bootstrap.

### Critério de avanço

Não avance para implantação completa se a infra estiver claramente bloqueada.

---

## Fase 4 — Estruturação do sistema de conhecimento

### Ação

O CKO contrata os agentes centrais de estruturação.

### Ordem recomendada

1. Knowledge Architect
2. Knowledge Librarian
3. Knowledge Discovery
4. Knowledge Curator
5. Knowledge Finder

### Checklist

- [ ] Knowledge Architect contratado
- [ ] Knowledge Librarian contratado
- [ ] Knowledge Discovery contratado
- [ ] Knowledge Curator contratado
- [ ] Knowledge Finder contratado
- [ ] Estrutura inicial da base definida
- [ ] Critérios de organização do acervo definidos
- [ ] Lista inicial de fontes prioritárias produzida
- [ ] Critérios de curadoria definidos
- [ ] Pelo menos um lote inicial de materiais aprovados incorporado

### Saída esperada

A organização já não está só com “papéis contratados”; existe base começando a ser montada de forma governada.

---

## Fase 5 — Governança de aprendizado

### Ação

Contratar o **Learning Manager**.

### Checklist

- [ ] Learning Manager contratado
- [ ] Protocolo de recebimento de aprendizados definido
- [ ] Critério de descarte definido
- [ ] Critério de memória revisável definido
- [ ] Critério de promoção para instrução permanente definido
- [ ] Pelo menos um aprendizado de teste processado

### Referência

- `agents/learning-manager.md`
- `templates/hire-learning-manager.md`

### Saída esperada

Aprendizados da operação deixam de ficar soltos e passam a ter governança.

---

## Fase 6 — Adoção operacional

### Ação

Contratar o **Knowledge Enablement**.

### Checklist

- [ ] Knowledge Enablement contratado
- [ ] Lista de agentes operacionais prioritários definida
- [ ] Pelo menos 1 agente operacional auditado
- [ ] Instrução de consultar base de conhecimento verificada
- [ ] Instrução de enviar aprendizados ao Learning Manager verificada
- [ ] Não conformidades documentadas
- [ ] Correções mínimas aplicadas nos agentes auditados

### Referência

- `agents/knowledge-enablement.md`
- `templates/hire-knowledge-enablement.md`

### Saída esperada

O sistema começa a ser usado por agentes reais, em vez de ficar só no desenho.

---

## Fase 7 — Avaliação inicial

### Ação

Contratar o **Knowledge Evaluator**.

### Checklist

- [ ] Knowledge Evaluator contratado
- [ ] Métricas ou sinais mínimos definidos
- [ ] Diagnóstico inicial produzido
- [ ] Lacunas prioritárias apontadas
- [ ] Gargalos iniciais apontados
- [ ] Feedback entregue ao CKO

### Referência

- `agents/knowledge-evaluator.md`
- `templates/hire-knowledge-evaluator.md`

### Saída esperada

A implantação passa a ser medida por utilidade real, não por percepção.

---

## Checklist de validação pós-contratação

Use esta seção depois que os agentes já estiverem contratados.

### Chief Knowledge Officer

- [ ] entende que lidera o time
- [ ] conhece a ordem de bootstrap
- [ ] sabe quais agentes contratar
- [ ] sabe quando escalar bloqueios

### Knowledge Infra

- [ ] validou AnythingLLM
- [ ] validou Paperclip/plugin/integrações
- [ ] consolidou bloqueios técnicos

### Knowledge Architect

- [ ] definiu estrutura inicial da base
- [ ] definiu organização lógica mínima

### Knowledge Librarian

- [ ] definiu rotina de higiene do acervo
- [ ] tem critério para redundância e obsolescência

### Knowledge Discovery

- [ ] produziu fontes candidatas
- [ ] alinhou foco por função ou domínio

### Knowledge Curator

- [ ] definiu o que entra e o que não entra
- [ ] priorizou conhecimento útil ao contexto real

### Knowledge Finder

- [ ] incorporou materiais aprovados
- [ ] registrou o que já foi obtido e ativado

### Learning Manager

- [ ] recebeu aprendizados de teste
- [ ] separou ruído, memória revisável e instrução permanente

### Knowledge Enablement

- [ ] auditou pelo menos um agente operacional
- [ ] encontrou e corrigiu lacunas de adoção

### Knowledge Evaluator

- [ ] gerou leitura inicial de impacto, lacunas e gargalos

---

## Papel de AnythingLLM, Paperclip e Learning Manager

### AnythingLLM

Trate como a camada de **consulta de conhecimento**.

Exemplos de uso:

- consultar repertório técnico
- consultar playbooks
- consultar documentos e referências
- apoiar decisões dos agentes operacionais

Não trate como substituto de instruções permanentes ou de governança.

### Paperclip

Trate como a camada **organizacional e operacional**.

É onde:

- os agentes são contratados
- os papéis existem
- a coordenação acontece
- o time opera no dia a dia

### Learning Manager

Trate como a camada de **governança do aprendizado novo**.

Ele evita dois erros comuns:

- transformar toda observação em regra permanente
- perder aprendizados úteis no meio da operação

---

## Teste mínimo de funcionamento real

Execute um piloto curto com 1 ou 2 agentes operacionais.

### Roteiro

- [ ] agente operacional recebe uma tarefa real
- [ ] agente consulta a base de conhecimento quando necessário
- [ ] agente identifica um aprendizado útil
- [ ] aprendizado é enviado ao Learning Manager
- [ ] Learning Manager processa esse aprendizado
- [ ] Knowledge Enablement verifica se o protocolo foi seguido
- [ ] Knowledge Evaluator registra o que funcionou e o que falhou

### Resultado esperado

Você consegue observar o ciclo completo:

**consulta → execução → aprendizado → governança → ajuste**

Se esse ciclo não fecha, o sistema ainda não está pronto.

---

## Erros de implantação mais comuns

- contratar vários agentes antes de validar infra
- pular a leitura do repositório e improvisar papéis
- usar AnythingLLM como substituto de governança
- ignorar o Learning Manager no início
- assumir adoção sem auditar agentes operacionais
- considerar o projeto pronto sem piloto real

---

## Ordem resumida de implementação

1. Contratar CKO
2. Mandar o CKO consultar o repositório
3. Contratar Knowledge Infra
4. Validar stack mínima
5. Contratar Architect, Librarian, Discovery, Curator e Finder
6. Ativar ingestão inicial
7. Contratar Learning Manager
8. Contratar Knowledge Enablement
9. Contratar Knowledge Evaluator
10. Rodar piloto real e corrigir lacunas
