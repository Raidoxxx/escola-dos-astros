# Escola dos Astros

Plataforma de gestão interna, colaboração e registro de participação acadêmica para apoiar as atividades do projeto Escola dos Astros.

## Objetivo

A proposta é centralizar em um único sistema o planejamento e a execução das atividades do projeto: eventos, observações, palestras, produção de conteúdo, reuniões, equipamentos e demais tarefas internas.

O sistema também deve permitir registrar o tempo dedicado por cada integrante, relacionar horas às atividades realizadas e gerar relatórios de participação.

> Esta documentação parte de oportunidades observadas externamente. Processos internos específicos da Escola dos Astros devem ser tratados como hipóteses até serem validados pela equipe responsável.

## Problema central

Projetos acadêmicos e de extensão podem envolver muitas atividades paralelas e pessoas diferentes. Quando tarefas, responsáveis, prazos, arquivos e horas ficam espalhados em conversas, planilhas ou anotações, torna-se difícil responder rapidamente:

- Quem está fazendo cada tarefa?
- O que está atrasado?
- O que falta para um evento acontecer?
- Quem está editando determinado vídeo?
- Quanto tempo cada integrante dedicou?
- Quais atividades contam para a participação acadêmica?
- Quais entregas comprovam essas horas?
- Como está a carga de trabalho da equipe?

O Escola dos Astros pretende transformar essas informações em um fluxo organizado e rastreável.

## Pilares

1. **Organização** — atividades, tarefas, responsáveis, prazos e agenda.
2. **Colaboração** — comunicação contextual, arquivos, decisões e acompanhamento.
3. **Participação acadêmica** — registro de tempo, metas de horas e relatórios.
4. **Comprovação** — evidências, entregas e validação quando necessária.
5. **Continuidade** — histórico e conhecimento que não se perdem quando integrantes mudam.

## MVP

O primeiro produto deve conter:

- autenticação e perfis;
- equipe e permissões;
- atividades/projetos;
- tarefas e subtarefas;
- responsáveis, prioridade, prazo e status;
- agenda;
- modelos reutilizáveis de atividades;
- pipeline de produção de conteúdo;
- cronômetro de trabalho;
- lançamento manual de horas;
- aprovação de horas manuais;
- metas de carga horária;
- anexos/evidências;
- dashboard individual;
- dashboard de coordenação;
- relatórios de participação;
- inventário básico de equipamentos.

## Exemplo de fluxo

```text
ATIVIDADE
   |
   +-- Planejamento
   +-- Tarefas
   +-- Responsáveis
   +-- Prazos
   +-- Equipamentos
   |
   v
EXECUÇÃO
   |
   +-- Trabalhar na tarefa
   +-- Registrar tempo
   +-- Anexar evidência
   +-- Concluir
   |
   v
VALIDAÇÃO
   |
   +-- Revisar entrega
   +-- Validar horas quando necessário
   |
   v
RELATÓRIOS
   |
   +-- Horas por integrante
   +-- Horas por atividade
   +-- Entregas realizadas
   +-- Participação por período
```

## Documentação

- [01 — Visão do produto](docs/01-visao-produto.md)
- [02 — Requisitos funcionais](docs/02-requisitos-funcionais.md)
- [03 — Fluxos e regras de negócio](docs/03-fluxos-e-regras.md)
- [04 — Horas e participação](docs/04-horas-e-participacao.md)
- [05 — Modelo conceitual de dados](docs/05-modelo-de-dados.md)
- [06 — Ideias e oportunidades](docs/06-ideias-e-oportunidades.md)
- [07 — Roadmap](docs/07-roadmap.md)
- [08 — Projeto de Extensão (PEX)](docs/08-pex.md)

## Status

**Fase atual:** planejamento do produto.

Ainda não foram definidas as tecnologias de implementação. A prioridade neste momento é entender o problema, delimitar o escopo e projetar os fluxos antes de iniciar o desenvolvimento.