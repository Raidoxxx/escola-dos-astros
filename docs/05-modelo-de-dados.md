# 05 — Modelo Conceitual de Dados

Este documento descreve entidades conceituais. O modelo físico do banco será definido somente após a escolha da arquitetura.

## Usuário

Campos sugeridos:

- id;
- nome;
- e-mail;
- função/vínculo;
- perfil de acesso;
- status;
- data de entrada;
- meta de horas opcional.

Relacionamentos:

- possui tarefas;
- participa de atividades;
- possui registros de tempo;
- pode validar registros conforme permissão;
- pode ficar responsável por equipamentos.

---

## Atividade

Representa um projeto, evento ou trabalho maior.

Campos:

- id;
- título;
- descrição;
- tipo;
- status;
- prioridade;
- data de início;
- data prevista de término;
- local;
- responsável principal;
- modelo de origem opcional;
- criado por;
- criado em.

Exemplos:

- Observação Astronômica — 18/09;
- Vídeo sobre Saturno;
- Visita à escola X;
- Reunião semanal;
- Manutenção dos telescópios.

---

## Participação em Atividade

Relaciona usuários e atividades.

Campos:

- usuário;
- atividade;
- papel na atividade;
- status da participação.

---

## Tarefa

Campos:

- id;
- atividade;
- tarefa pai opcional;
- título;
- descrição;
- status;
- prioridade;
- responsável principal;
- prazo;
- estimativa de minutos;
- criada por;
- criada em;
- concluída em.

---

## Responsável de Tarefa

Caso seja necessário permitir múltiplos responsáveis:

- tarefa;
- usuário;
- tipo de responsabilidade.

---

## Dependência de Tarefa

- tarefa bloqueada;
- tarefa necessária.

Exemplo:

```text
Gravação depende de Roteiro aprovado
Edição depende de Gravação concluída
```

---

## Registro de Tempo

Campos:

- id;
- usuário;
- atividade;
- tarefa opcional;
- origem: cronômetro/manual/presença;
- início opcional;
- fim opcional;
- duração em minutos;
- descrição;
- status;
- criado em;
- atualizado em.

---

## Validação de Tempo

Campos:

- registro de tempo;
- validador;
- decisão;
- comentário;
- data.

---

## Evidência

Campos:

- id;
- tipo;
- URL ou referência de arquivo;
- descrição;
- tarefa opcional;
- registro de tempo opcional;
- enviado por;
- criado em.

---

## Comentário

- id;
- autor;
- tarefa ou atividade;
- conteúdo;
- criado em;
- editado em.

---

## Modelo de Atividade

Campos:

- id;
- nome;
- descrição;
- tipo;
- ativo.

Possui uma lista de tarefas-modelo.

---

## Tarefa de Modelo

- modelo;
- título;
- descrição;
- ordem;
- categoria;
- prazo relativo opcional;
- dependência opcional.

---

## Equipamento

Campos:

- id;
- nome;
- categoria;
- patrimônio/código opcional;
- descrição;
- estado;
- observações.

---

## Reserva de Equipamento

- equipamento;
- atividade;
- responsável;
- início;
- fim previsto;
- devolvido em;
- estado na retirada;
- estado na devolução.

---

## Evento de Agenda

Pode representar reunião, evento ou compromisso que não justifique uma atividade completa.

Campos:

- id;
- título;
- início;
- fim;
- local;
- descrição;
- atividade relacionada opcional.

---

## Presença

Possível entidade para reuniões e eventos internos.

Campos:

- evento;
- usuário;
- status;
- horário de entrada opcional;
- horário de saída opcional;
- confirmado por.

---

## Conteúdo

Para o fluxo editorial:

- id;
- título;
- tipo;
- etapa;
- atividade relacionada;
- data planejada de publicação;
- link publicado;
- responsável atual.

---

## Ata / Decisão

Possível módulo leve para reuniões.

Campos:

- reunião;
- resumo;
- decisão;
- autor;
- data.

Decisões podem gerar tarefas.

---

## Notificação

- destinatário;
- tipo;
- título;
- mensagem;
- referência de contexto;
- lida em.

---

# Relação simplificada

```text
USUÁRIO
  ├──< TAREFA
  ├──< REGISTRO_DE_TEMPO >── ATIVIDADE
  ├──< PARTICIPAÇÃO >──────── ATIVIDADE
  └──< PRESENÇA >──────────── EVENTO

ATIVIDADE
  ├──< TAREFA
  ├──< RESERVA >───────────── EQUIPAMENTO
  ├──< CONTEÚDO
  └──< EVENTO

TAREFA
  ├──< EVIDÊNCIA
  ├──< COMENTÁRIO
  └──< REGISTRO_DE_TEMPO
```

## Observação

No MVP, algumas dessas entidades podem ser simplificadas. Este documento existe para evitar decisões precoces e preservar espaço para evolução.