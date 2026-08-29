# 03 — Fluxos e Regras de Negócio

## Fluxo 1 — Criar uma atividade

```text
Coordenação cria atividade
        ↓
Define tipo, data e responsável
        ↓
Escolhe modelo (opcional)
        ↓
Sistema cria tarefas padrão
        ↓
Responsáveis são atribuídos
        ↓
Atividade entra em planejamento
```

### Regras

- uma atividade pode existir sem data final definida;
- uma atividade pode ter vários integrantes;
- tarefas podem possuir responsáveis diferentes;
- modelos não devem impedir edição posterior das tarefas criadas.

---

## Fluxo 2 — Executar uma tarefa

```text
Integrante recebe tarefa
        ↓
Consulta descrição e prazo
        ↓
Inicia trabalho
        ↓
Registra tempo
        ↓
Adiciona comentário/evidência
        ↓
Envia para revisão ou conclui
```

### Regras

- uma tarefa bloqueada deve informar o motivo;
- uma tarefa vencida e não concluída deve ser identificada como atrasada;
- conclusão não apaga o histórico de horas, comentários ou arquivos;
- quando houver revisão obrigatória, o responsável não deve validar a própria entrega se a política do projeto exigir revisão externa.

---

## Fluxo 3 — Produção de vídeo

```text
Ideia
  ↓
Pesquisa
  ↓
Roteiro
  ↓
Revisão do roteiro
  ↓
Gravação
  ↓
Edição
  ↓
Revisão final
  ↓
Publicação
```

Cada etapa pode gerar uma tarefa independente, com responsáveis e horas próprias.

### Exemplo

```text
Vídeo: Por que Saturno tem anéis?

Pesquisa       Maria     1h20
Roteiro        João      2h10
Gravação       Ana       1h30
Edição         Lucas     4h15
Revisão        Maria     0h40
--------------------------------
Total                    9h55
```

---

## Fluxo 4 — Evento/observação

```text
Planejamento
   ↓
Definição de equipe
   ↓
Reserva de equipamentos
   ↓
Preparação de materiais
   ↓
Realização
   ↓
Registro de participação
   ↓
Organização de arquivos
   ↓
Conteúdo/relatório pós-evento
```

### Checklist reutilizável sugerido

- confirmar data;
- confirmar local;
- definir equipe;
- verificar previsão do tempo, quando aplicável;
- separar equipamentos;
- conferir equipamentos;
- preparar materiais;
- criar divulgação;
- realizar atividade;
- registrar presença da equipe;
- armazenar fotos e arquivos;
- registrar resultados;
- devolver equipamentos;
- criar conteúdo pós-evento.

---

## Fluxo 5 — Registro de horas

### Cronômetro

```text
Abrir tarefa
   ↓
Iniciar cronômetro
   ↓
Pausar/continuar conforme necessário
   ↓
Finalizar
   ↓
Registro associado à tarefa
```

### Registro manual

```text
Adicionar registro
   ↓
Informar tarefa, data, duração e descrição
   ↓
Anexar evidência quando necessário
   ↓
Enviar
   ↓
Aguardando validação
   ↓
Aprovado ou devolvido para correção
```

---

## Fluxo 6 — Reunião

Uma reunião pode ser tratada como uma atividade própria.

O sistema pode registrar:

- data;
- participantes;
- pauta;
- duração;
- decisões;
- tarefas geradas;
- responsáveis;
- prazos.

### Resultado esperado

```text
REUNIÃO
   ↓
DECISÕES
   ↓
TAREFAS
   ↓
RESPONSÁVEIS
```

Isso reduz a perda de decisões tomadas apenas verbalmente.

---

# Regras Gerais

## RN-001 — Rastreabilidade

Alterações importantes devem preservar histórico quando afetarem participação acadêmica, especialmente:

- alteração de horas;
- aprovação/rejeição;
- troca de responsável;
- conclusão/reabertura de tarefa.

## RN-002 — Exclusão

Registros que possuem valor acadêmico não devem ser eliminados silenciosamente. Preferir arquivamento ou exclusão com auditoria.

## RN-003 — Horas simultâneas

O sistema não deve permitir dois cronômetros ativos para o mesmo integrante no mesmo período.

## RN-004 — Duração inválida

Registros com duração zero ou negativa são inválidos.

## RN-005 — Registros extensos

O sistema pode sinalizar registros excepcionalmente longos para revisão, sem assumir automaticamente fraude.

## RN-006 — Metas de horas

Meta de horas é um indicador de acompanhamento, não deve calcular automaticamente nota acadêmica sem que a regra oficial de avaliação seja conhecida e configurada.

## RN-007 — Evidência

A exigência de evidência pode variar conforme o tipo de tarefa.

Exemplos:

- edição: arquivo ou link do vídeo;
- roteiro: documento;
- evento presencial: confirmação de participação;
- reunião: presença/ata;
- organização de equipamento: confirmação do responsável.

## RN-008 — Privacidade

Evitar cadastrar dados pessoais de público externo quando não forem necessários à finalidade do sistema.

## RN-009 — Atividades recorrentes

Modelos podem ser reutilizados para criar atividades recorrentes sem duplicar manualmente todo o checklist.

## RN-010 — Responsabilidade coletiva

Uma atividade pode ter várias pessoas, mas tarefas importantes devem deixar claro quem é o responsável principal.