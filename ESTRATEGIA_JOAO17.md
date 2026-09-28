# Estratégia — Pesquisa Ampla, Profunda e Detalhada sobre João 17

*v2, 28/09/2026. A v1 deste documento foi escrita a partir de quatro artefatos
do projeto-mãe (`CLAUDE.md`, `CHECKPOINT_PROJETO.md`, `AQUISICOES_ESCOLAS.md`,
`AQUISICOES_LACUNAS.md`) e presumia que o Capítulo 17 ainda não tinha sido
trabalhado na Fase 2. **Essa presunção estava errada**, e cinco arquivos novos
(`CURADORIA_FONTES_JOAO.md`, `DEEP_RESEARCHES_JOAO.md`,
`LACUNAS_REFUTACAO.md`, `LOG_QUERIES.md`, `MEMORIA_PROJETO.md`) a corrigem.
Esta versão não descarta a v1 — a estrutura em três blocos, as sentinelas e o
padrão de cinco itens continuam válidos — mas reposiciona o projeto a partir
do estado real, não do presumido.*

---

## 0. O que mudou, e por que muda a missão deste repositório

**João 17 já foi trabalhado, entregue e podado.** Do `MEMORIA_PROJETO.md`
(atualizado 21-23/09/2026):

| Item | Estado real, medido |
|---|---|
| Notebook | `Joao - Cap17 (Oração Sacerdotal)` — `575759eb-237e-44b4-8c72-092eb20ba656` |
| Relatório | **Entregue em 11/09/2026** — `_entregas/Relatorio_Cap17_Joao.md/.docx/.pdf` |
| Corpus | Chegou a **327 fontes** (300 `ready`), depois **poda semântica em 21/09**: 300 → **176** (125 `ISOLADA` removidas, ficaram 25 sem status) |
| Deep Research | **9 de 10 rodadas** executadas (5 lacunas × 2 rodadas) |
| Triagem semântica | R1/R2/R3 rodados **do zero em 21/09** (corrigindo a nota anterior, de 12/09, que dizia "nunca rodou") — ledger **36/36** completo |
| Refutações já registradas no relatório entregue | **(a)** heterodoxias sobre 17.5 — unitarismo, modalismo, arianismo — pelo padrão de 5 itens; **(b)** uso ecumênico-institucional de 17.21 (citando nominalmente ***Ut Unum Sint***) — também pelo padrão de 5 itens completo |
| Estúdio (áudio/vídeo) | Campanha de 60 queries planejadas (5 destaques × 6 personas × 2 formatos); **49 disparadas, 0 confirmadas como artefato real** (log gerado em modo offline, sem `artifact list`); **11 nunca chegaram a ser disparadas** |

Isto muda a pergunta que este repositório responde. **Não é mais "como
executar a exegese de João 17 pela primeira vez"** — isso já aconteceu, e com
qualidade registrada (o par de refutações de 17.5 e 17.21 é descrito no
`MEMORIA_PROJETO.md` como *"a mais completa aplicação da Regra Zero do
projeto"*, dito do Cap. 20, mas o Cap. 17 é citado com o mesmo padrão de
detalhe). **A pergunta correta é: o que um capítulo entre 21, sob o teto de
formato da Fase 2, não pôde comportar — e que uma obra dedicada,
exclusivamente sobre João 17, pode?**

Um capítulo de série tem: um relatório de poucas páginas, um corpus podado
para caber ao lado de outros 20 capítulos, cinco prompts exegéticos, e uma
Estúdio que sequer terminou de disparar. Este projeto (`joao17`) tem a
liberdade que a série não tem — o espaço para tratar o texto com a extensão,
polêmica e detalhe que ele pede, sem competir por atenção com Nicodemos ou o
Bom Pastor.

---

## 1. As quatro tarefas concretas que decorrem disso

### 1.1 Auditar o que já foi entregue (prioridade imediata, é a mais barata)

Antes de escrever uma linha nova, ler o `Relatorio_Cap17_Joao.md` já entregue
e aplicar-lhe as mesmas checagens que o projeto-mãe já provou serem
necessárias em outros capítulos — porque **nenhuma checagem específica de
Jo 17 foi registrada, só as gerais do fluxo**:

- **Conferir citação por citação** (`conferir_citacoes.py`), como foi feito
  para os 121 da Fase 1 — não há registro de que a Fase 2 tenha rodado o
  mesmo conferidor sobre os relatórios de capítulo.
- **Verificar se as 25 fontes "sem status"** que sobraram da poda de 21/09
  (nem `ISOLADA` nem `CONFLITO`) foram lidas e usadas, ou são passageiras
  silenciosas — a mesma checagem de presença-sem-cobertura que a v1 já exigia
  para Bengel e Wesley.
- **Confirmar a fonte primária por trás de *Ut Unum Sint*** citada no
  relatório: é encíclica real (João Paulo II, 1995) sobre compromisso
  ecumênico — mas conferir **edição, parágrafo exato citado, e se o
  relatório cita o documento em fonte primária ou por resumo de terceiro**
  (a Regra 12 do projeto-mãe: nome de obra não é evidência de que foi lida).
- **Rodar a Sentinela 17-A proposta na v1** (P66 cobre só até 14.26; P75 só
  até 15.8 — nenhum dos dois cobre Jo 17) contra o texto entregue: confirmar
  que nenhuma alegação de suporte papiráceo antigo foi feita para este
  capítulo. Não há registro de que essa sentinela específica tenha sido
  conferida — é sentinela nova, proposta por este repositório, não herdada.

### 1.2 Fechar o Estúdio — é trabalho começado e abandonado no meio

Dos 60 áudios/vídeos planejados, **49 foram disparados e nenhum foi
confirmado**, porque o log de 27/09 foi gerado em modo offline (sem
`artifact list`). Isto é exatamente o tipo de situação que o
`MEMORIA_PROJETO.md` já alertou ser enganosa: *"nunca aceitar `rc!=0` de
`generate` como falha — sempre conferir por `artifact list --json`"*. Antes
de decidir se os 49 precisam ser re-disparados, **conferir via `artifact
list`** quantos de fato existem — pode ser que boa parte já esteja pronta e
só não tenha sido reconciliada.

As **11 sem registro de disparo** (dos 60 planejados) precisam ser
localizadas no script `fase2-capitulos/cap17-oracao-sacerdotal/estudio_cap17.py`
e disparadas.

### 1.3 Ir além do que o formato de capítulo permitiu

Com a auditoria feita, a contribuição real deste projeto dedicado é
**aprofundar além do que um relatório de capítulo-entre-21 comporta**. Onde a
v1 já mapeava isso corretamente (estrutura em três blocos, sentinelas,
escolas de interpretação), a diferença agora é que não se está mais
preenchendo lacuna nenhuma — está-se **expandindo um trabalho já bem-feito em
formato reduzido**. As frentes concretas de expansão, cruzando o que a
`CURADORIA_FONTES_JOAO.md` já cataloga:

| Frente de expansão | Por que o capítulo-padrão não comportou | Fonte já disponível para isso |
|---|---|---|
| **Recepção patrística plena de Jo 17** | 5 prompts exegéticos por capítulo não dão espaço para percorrer Orígenes, Crisóstomo, Cirilo e Agostinho versículo a versículo sobre a Oração; um capítulo-padrão cita, não expõe | Orígenes, Agostinho (*Tractates*), Cirilo (2 vols.), ACCS 11-21 — todos Tier A/S já no corpus geral |
| **Gênero literário da oração sacerdotal em profundidade** | é tema transversal (herdado do Cap. 6, discurso de despedida) que nenhum capítulo isolado pode tratar por inteiro | Segovia, Kurz (lacunas já identificadas para o Cap. 6 em `AQUISICOES_LACUNAS.md`) — aqui podem finalmente receber tratamento completo |
| **O debate calvinista-arminiano sobre 17.9-12** | a Estúdio já roteirizou isso como debate de personas (query D1P4 acima, calvinista × arminiano sobre 17.5) mas o relatório de capítulo não tem espaço para desenvolver as duas posições com igual profundidade | Ridderbos/Calvino (reformado) vs. Wesley/Clarke (arminiano-wesleyano) — ambos no corpus |
| **A tradição expositiva reformada dedicada a Jo 17** | Lloyd-Jones (*Tier C* na `CURADORIA_FONTES_JOAO.md`, mas nominalmente marcado como "**excelente para o cap. 17**") é a única obra do corpus **inteiramente dedicada** a este capítulo, e um relatório padrão não a esgota | Lloyd-Jones, *João 17* — já no acervo |
| **Teologia trinitária da reciprocidade Pai-Filho** | 17.1-5, 17.21-23 e 17.24-26 sustentam boa parte da doutrina histórica de *perichoresis*; um capítulo de série não tem espaço para a história dogmática (Niceia, Constantinopla, disputas cristológicas patrísticas) | Cirilo de Alexandria (anti-arianismo), Agostinho (*De Trinitate* — já no acervo geral do projeto-mãe) |

### 1.4 Verificar o que a Pauta 1 de refutação (gênero/feminismo) não cobriu

`LACUNAS_REFUTACAO.md` registra a Pauta 1 (hermenêutica feminista) como
incidindo em Jo 2.4, 4, 11.27 e 20.11-18 — **não em Jo 17**. Isto é
verificação negativa útil: não há objeção de gênero pendente específica
deste capítulo, e não se deve importar uma artificialmente. Onde Jo 17 toca
o mesmo eixo é indiretamente, pela intercessão sacerdotal e a tipologia de
Cristo como sumo sacerdote (papel tradicionalmente masculino no AT) — mas
isso é ponto de **cristologia**, não de objeção de gênero ao texto, e não
deve ser tratado como se fosse.

---

## 2. O que a v1 já estabeleceu e continua valendo, sem alteração

- **A estrutura em três blocos concêntricos** (17.1-5 / 17.6-19 / 17.20-26) —
  confirmada, de resto, pela própria Estúdio já roteirizada: as queries D1
  giram em torno de 17.1-5 exatamente como a v1 previu.
- **A Regra Zero aplicada à leitura ecumênica de 17.21-23** — confirmada como
  o eixo mais sensível do capítulo: é justamente o que o relatório já
  entregue tratou como refutação de destaque (§0 acima).
- **A distinção entre objeção externa (ecumênica) e debate interno
  (calvinista × arminiano)** sobre 17.9-12 — confirmada pela própria Estúdio,
  que roteiriza esse debate como **duas vozes do campo confessional em
  diálogo**, não como refutação de uma pelas outra.
- **A Sentinela 17-A** (P66/P75 não cobrem Jo 17) — proposta na v1, ainda não
  verificada contra o texto entregue. Ver §1.1.

---

## 2-B. Achados dos cinco arquivos de base (`PLANO_JOAO`, `REGRAS_RETOMADA`,
`REVISAO_LACUNAS`, `ROTEIRO_VERSIONAMENTO`, `Sequencia_Notebook_Joao`)

São documentos de fundação e processo (o plano original de 24/07, as regras
gerais de retomada, uma auditoria de lacunas restrita aos capítulos 1-9, e um
roteiro técnico de versionamento). Não trazem lacuna nova de Jo 17 — a
`REVISAO_LACUNAS.md` é explícita: cobre só os caps. 1-9. Mas confirmam ou
acrescentam três pontos que valem registro:

1. **Lloyd-Jones, *João 17*, são 4 volumes — não um só.**
   `Sequencia_Notebook_Joao.md` (linha 216) lista a obra entre o que foi
   **deliberadamente excluído do notebook da Fase 1**, junto com as demais
   monografias reservadas para entrar "no Deep Research da Fase 2" — ou seja,
   desde a montagem do corpus em 24-25/07 já se previa que este seria **o**
   texto reformado dedicado ao capítulo. Isso eleva o peso da frente de
   expansão §1.3 ("a tradição expositiva reformada dedicada a Jo 17"): 4
   volumes de exposição pastoral-teológica dão material real para a leitura
   plena que um relatório de capítulo-entre-21 não pôde esgotar. **Conferir
   quantos dos 4 volumes efetivamente entraram no corpus do notebook
   `575759eb`** — o inventário desta sessão não permite saber; é item de
   auditoria a somar ao §1.1.
2. **O padrão de cinco itens e as sentinelas gerais, confirmados sem
   alteração.** `REGRAS_RETOMADA.md` §3 e §6 reproduzem exatamente o que a v1
   já assumia (nenhuma sentinela específica de Jo 17 aparece nestes
   documentos além da 17-A já proposta aqui) — não há retrabalho a fazer
   nesse ponto.
3. **O projeto-mãe, em 01/08/2026, não tinha remoto git** —
   `ROTEIRO_VERSIONAMENTO.md` confirma repositório só local, com espelho
   manual no Google Drive, "fotografia" que não sincroniza sozinha. Isto é
   relevante para este repositório (`joao17`), que **tem** remoto no GitHub:
   qualquer arquivo do projeto-mãe que se queira trazer para cá (o
   `Relatorio_Cap17_Joao.md` já entregue, por exemplo) precisa ser copiado
   manualmente pelo usuário — não há como este repositório buscá-lo sozinho.

---

## 3. Plano de execução revisado

| Ordem | Tarefa | Depende de |
|---|---|---|
| 1 | `artifact list --json` no notebook `575759eb` — reconciliar os 49 disparos do Estúdio contra artefatos reais | acesso ao ambiente Windows/NotebookLM do projeto-mãe (fora deste repositório) |
| 2 | Disparar as 11 queries do Estúdio sem registro | idem |
| 3 | Ler `Relatorio_Cap17_Joao.md` na íntegra e rodar `conferir_citacoes.py` sobre ele | acesso ao arquivo entregue (não incluído nos uploads desta sessão — solicitar) |
| 4 | Verificar a Sentinela 17-A contra o texto entregue | idem |
| 5 | A partir da auditoria, decidir com o usuário **quais das quatro frentes de expansão (§1.3)** valem o investimento de uma obra dedicada, e em que ordem | resultado de 1-4 |

**Nota de escopo para este repositório (`joao17`):** ele não tem acesso ao
ambiente Windows do projeto-mãe (NotebookLM, `biblioteca/`, os scripts
PowerShell) — é um ambiente cloud isolado. O que pode ser feito aqui é
**planejamento, auditoria de texto já fornecido, e redação** — não execução
de `notebooklm` ou disparo de Estúdio. Qualquer item acima que exija esses
recursos precisa ser executado na janela do projeto-mãe e trazido de volta
como artefato (relatório, log) para leitura e auditoria aqui.

---

## 4. Entregável revisado

Não mais um único `Relatorio_Cap17_Joao.md` — esse já existe. O entregável
deste repositório é uma **obra ampliada e dedicada**, provisoriamente
`Joao17_Estudo_Ampliado.md`, estruturada como:

1. **Auditoria do relatório existente** (§1.1) — correções, se houver.
2. **Os três blocos exegéticos**, cada um agora com o espaço que a série não
   deu: patrística plena, debate calvinista-arminiano nas duas vozes,
   gênero da oração sacerdotal, teologia trinitária da reciprocidade.
3. **Apêndice de sentinelas e checkpoint factual**, incluindo a 17-A.
4. **Registro do que continua sendo apenas do projeto-mãe** — Estúdio,
   notebook, poda — para não duplicar controle de estado em dois lugares.
