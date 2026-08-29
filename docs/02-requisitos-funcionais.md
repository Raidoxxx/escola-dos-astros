# 02 — Requisitos Funcionais

## Perfis e acesso

### RF-001 — Autenticação
O sistema deve permitir login seguro para integrantes autorizados.

### RF-002 — Perfis
Cada integrante deve possuir nome, vínculo/função, status e informações necessárias ao acompanhamento interno.

### RF-003 — Permissões
O sistema deve diferenciar, no mínimo:

- integrante;
- coordenador/administrador.

Permissões mais específicas podem ser adicionadas depois.

---

## Atividades e projetos

### RF-010 — Criar atividade
Permitir criar uma atividade com:

- título;
- descrição;
- tipo;
- data de início;
- data prevista de término;
- local, quando aplicável;
- responsável geral;
- participantes da equipe;
- status;
- prioridade.

### RF-011 — Status de atividade
Sugestão inicial:

- planejamento;
- em andamento;
- aguardando;
- concluída;
- cancelada.

### RF-012 — Modelos de atividade
Permitir criar uma atividade a partir de um modelo reutilizável.

Exemplos:

- observação astronômica;
- palestra;
- produção de vídeo;
- visita escolar;
- oficina.

Ao usar um modelo, tarefas padrão podem ser criadas automaticamente.

---

## Tarefas

### RF-020 — Criar tarefas e subtarefas
Cada tarefa pode possuir:

- título;
- descrição;
- responsável;
- prazo;
- prioridade;
- status;
- estimativa de tempo;
- tags;
- anexos;
- atividade associada.

### RF-021 — Status de tarefa
Sugestão:

- a fazer;
- em andamento;
- aguardando revisão;
- bloqueada;
- concluída.

### RF-022 — Dependências
Uma tarefa poderá depender de outra.

Exemplo:

```text
Roteiro aprovado
      ↓
Gravação
      ↓
Edição
      ↓
Publicação
```

### RF-023 — Responsabilidade
Uma tarefa deve possuir pelo menos um responsável principal quando entrar em execução.

### RF-024 — Comentários
Integrantes devem poder registrar comentários contextualizados dentro da tarefa.

### RF-025 — Evidências
Uma tarefa pode receber evidências como:

- arquivo;
- imagem;
- link;
- texto explicativo.

---

## Produção de conteúdo

### RF-030 — Pipeline editorial
Conteúdos devem poder percorrer etapas como:

- ideia;
- pesquisa;
- roteiro;
- gravação;
- edição;
- revisão;
- agendado;
- publicado.

### RF-031 — Conteúdo vinculado a atividade
Um vídeo ou publicação pode estar relacionado a um evento ou projeto maior.

### RF-032 — Responsáveis por etapa
Cada etapa pode ser atribuída a uma pessoa diferente.

---

## Agenda

### RF-040 — Calendário
Exibir atividades, tarefas com prazo, reuniões e eventos em calendário.

### RF-041 — Visões
Prever visualização por:

- dia;
- semana;
- mês.

### RF-042 — Minha agenda
Cada integrante deve poder filtrar apenas compromissos relevantes para si.

---

## Controle de horas

### RF-050 — Cronômetro
Integrante deve poder iniciar, pausar, continuar e finalizar um registro de trabalho ligado a uma tarefa.

### RF-051 — Registro manual
Permitir lançamento manual de horas com:

- data;
- duração;
- atividade/tarefa;
- descrição;
- evidência opcional ou obrigatória conforme regra.

### RF-052 — Aprovação
Registros manuais podem ficar pendentes até validação da coordenação.

### RF-053 — Meta de horas
Permitir configurar uma carga horária esperada por integrante ou período.

### RF-054 — Histórico
Integrante deve visualizar todo o histórico de horas registradas e o status de cada registro.

### RF-055 — Correções
Alterações em registros já aprovados devem manter rastreabilidade.

---

## Equipe

### RF-060 — Painel de membros
Exibir integrantes ativos, tarefas atuais e indicadores básicos de carga de trabalho.

### RF-061 — Minha semana
Cada integrante deve possuir uma visão simples contendo:

- tarefas de hoje;
- tarefas da semana;
- atrasadas;
- próximos eventos;
- horas no período.

### RF-062 — Disponibilidade
Evolução possível: permitir que integrantes indiquem indisponibilidades ou horários preferenciais.

---

## Equipamentos

### RF-070 — Inventário
Cadastrar equipamentos relevantes, como telescópios, câmeras, tripés e projetores.

### RF-071 — Reserva/vínculo
Vincular equipamentos a uma atividade.

### RF-072 — Responsável
Registrar quem ficou responsável por transportar ou devolver determinado item.

### RF-073 — Estado do equipamento
Registrar estados como:

- disponível;
- reservado;
- em uso;
- manutenção;
- indisponível.

---

## Relatórios

### RF-080 — Relatório individual
Gerar resumo por integrante com:

- horas registradas;
- horas aprovadas;
- tarefas concluídas;
- atividades participadas;
- distribuição das horas por categoria.

### RF-081 — Relatório por período
Filtrar dados por semana, mês, semestre ou intervalo personalizado.

### RF-082 — Relatório por atividade
Mostrar esforço total dedicado a uma atividade e por quem.

### RF-083 — Exportação
Evolução desejada: exportar relatórios em PDF e CSV.

---

## Dashboard

### RF-090 — Dashboard do integrante
Mostrar:

- minhas tarefas;
- horas realizadas;
- meta de horas;
- atividades próximas;
- pendências.

### RF-091 — Dashboard da coordenação
Mostrar:

- tarefas em andamento;
- tarefas atrasadas;
- atividades da semana;
- registros de horas pendentes;
- carga de trabalho da equipe;
- equipamentos reservados;
- conteúdos em produção.

---

## Notificações

### RF-100 — Notificações internas
Notificar sobre eventos importantes, como:

- nova tarefa atribuída;
- prazo próximo;
- tarefa atrasada;
- comentário ou menção;
- horas aprovadas/rejeitadas;
- atividade alterada.

Integrações externas ficam para versões futuras.