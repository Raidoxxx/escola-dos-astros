# 04 — Horas e Participação

## Objetivo

O controle de horas deve registrar quanto tempo cada integrante dedica ao projeto e, principalmente, **em que esse tempo foi utilizado**.

Como a participação pode ter impacto acadêmico, o módulo precisa ser simples para quem registra e confiável para quem acompanha.

## Formas de registro

### 1. Cronômetro

Fluxo recomendado:

```text
Abrir tarefa
→ Iniciar
→ Pausar/continuar
→ Finalizar
→ Revisar registro
→ Salvar
```

Dados mínimos:

- integrante;
- tarefa;
- atividade;
- início;
- fim;
- duração;
- descrição opcional.

### 2. Registro manual

Necessário para atividades em que o integrante esqueceu de iniciar o cronômetro ou trabalhou fora do sistema.

Campos:

- data;
- duração;
- atividade/tarefa;
- descrição do que foi realizado;
- evidência quando aplicável;
- justificativa opcional.

Sugestão: registros manuais entram como **pendentes de validação**.

## Status de um registro

- rascunho;
- pendente;
- aprovado;
- devolvido para correção;
- rejeitado;
- cancelado.

## Evidências

Nem toda atividade precisa de arquivo, mas o sistema deve permitir comprovação contextual.

Possíveis evidências:

- arquivo;
- link;
- imagem;
- comentário do coordenador;
- tarefa concluída;
- presença em atividade;
- ata de reunião.

## Meta de horas

O sistema pode possuir metas configuráveis por período.

Exemplo:

```text
Carga esperada: 60h
Horas aprovadas: 43h20
Horas pendentes: 2h30
Progresso aprovado: 72%
Faltam: 16h40
```

A meta deve ser apenas uma referência configurável até que a regra acadêmica oficial seja conhecida.

## Dashboard individual

Deve mostrar, no mínimo:

- horas aprovadas no período;
- horas pendentes;
- meta;
- progresso percentual;
- últimas atividades;
- distribuição de horas por categoria;
- tarefas que ainda precisam de evidência ou revisão.

## Dashboard da coordenação

Exemplo:

```text
PARTICIPAÇÃO — AGOSTO

Lucas    18h40 aprovadas   2h pendentes
Maria    16h15 aprovadas   0h pendentes
João     13h50 aprovadas   1h30 pendentes
Ana      11h20 aprovadas   0h pendentes
```

Filtros úteis:

- integrante;
- período;
- categoria;
- atividade;
- status da validação.

## Distribuição por categoria

Categorias iniciais sugeridas:

- eventos;
- reuniões;
- pesquisa;
- roteiro;
- gravação;
- edição;
- design;
- divulgação;
- equipamentos;
- documentação;
- organização interna;
- treinamento.

Exemplo:

```text
Lucas — Agosto

Edição                     6h20
Observações/Eventos        4h00
Reuniões                   2h30
Roteiro/Pesquisa           2h10
Equipamentos               1h40
Outras                     2h00
-------------------------------
Total                     18h40
```

## Relatório individual

O sistema deve ser capaz de produzir um extrato contendo:

- nome do integrante;
- período;
- total registrado;
- total aprovado;
- total pendente;
- lista de atividades;
- tarefas concluídas;
- horas por categoria;
- evidências associadas;
- validações realizadas.

## Auditoria

Para proteger a confiabilidade do histórico:

- registrar quem aprovou ou rejeitou horas;
- registrar data da validação;
- preservar valor anterior quando um registro aprovado for alterado;
- impedir sobreposição de cronômetros;
- sinalizar durações incomuns;
- não permitir alteração silenciosa de registros consolidados.

## Ideia futura — presença automática

Uma evolução possível é registrar presença em eventos/reuniões e sugerir uma entrada de horas automaticamente.

Exemplo:

```text
Reunião semanal
14:00–15:20

Presença confirmada: João

[Sugerir registro de 1h20]
```

A pessoa ainda revisaria o registro antes da confirmação.

## Ideia futura — comparação entre estimado e realizado

Tarefas podem ter estimativa de tempo.

```text
Editar vídeo
Estimado: 3h
Realizado: 4h20
```

Isso ajuda o projeto a melhorar o planejamento sem transformar a ferramenta em mecanismo de cobrança excessiva.