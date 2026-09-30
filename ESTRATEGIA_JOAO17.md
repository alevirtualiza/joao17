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

### 1.1-B Auditoria executada em 28/09/2026 — o texto do relatório foi lido

O usuário enviou `Relatorio_Cap17_Joao.md` (6 seções + notação de certeza,
datado 11/09/2026). Isto permite fechar boa parte de §1.1 de fato, não só
planejá-la. Resultado, item por item:

**✅ Sentinela 17-A — sem violação.** O relatório não invoca P66 nem P75 em
nenhum ponto para sustentar o texto de Jo 17 — não há qualquer alegação de
suporte papiráceo antigo para este capítulo. A crítica textual do capítulo
simplesmente não é tratada (nem para afirmar, nem para negar cobertura
manuscrita) — o que é consistente com a sentinela, mas também deixa uma
lacuna honesta: **nenhuma seção trata os testemunhos textuais de Jo 17**
(quais unciais o cobrem, se há variante relevante). Candidato a frente de
expansão adicional, não previsto na v1: uma nota de crítica textual do
capítulo, ausente do relatório por decisão editorial ou por lacuna real —
não há como saber qual das duas pelo texto sozinho.

**✅ *Ut Unum Sint* — citada como deveria.** O relatório nomeia a encíclica,
*Unitatis Redintegratio* e documentos do CMI como fonte primária da
objeção ecumênica, e cumpre os cinco itens explicitamente rotulados
(1)-(5) no corpo do texto — é, de fato, a aplicação mais completa e
explícita do padrão neste relatório. Falta apenas o dado bibliográfico
fino (edição, parágrafo) que só se confere no documento original — fora
do alcance deste repositório.

**⚠️ Achado: rótulo de certeza contraditório em si mesmo (17.5).** O
relatório define, na sua própria escala, `HP` = *"hipótese plausível —
sem consenso, mas **sem objeção séria conhecida**"* e `HR` = *"hipótese
refutada — proposta exposta e, em seguida, **demonstrada improcedente
neste relatório**"*. Mas a frase que trata as leituras unitária/sociniana,
modalista e ariana de 17.5 diz: *"foram apresentadas com fonte e
classificadas ^HP^; **refutadas** porque (1)... (2)... (3)..."* — no mesmo
parágrafo em que as declara refutadas, rotula-as com o selo que por
definição significa "sem objeção séria". Pela própria escala do relatório,
deveriam levar `^HR^`, não `^HP^`. É exatamente o tipo de erro que o
projeto-mãe já corrigiu antes (rótulo inflado ou mal-aplicado — ver a
auditoria do Cap. 1 em `CLAUDE.md` §2-B) — aqui não infla a tese, mas
descreve mal a própria refutação que o texto acabou de fazer.

✅ **Corrigido em 28/09/2026** — `^HP^` trocado por `^HR^` na cópia
enviada a esta sessão (`.../uploads/.../7d4a63a4-Relatorio_Cap17_Joao.md`).
✅ **Fechado em 28/09/2026** — o usuário reenviou o `.md` de origem;
corrigido de novo (o upload chegou sem a edição anterior, como esperado —
uploads não se sincronizam entre si) e devolvido via `SendUserFile` como
`Relatorio_Cap17_Joao_CORRIGIDO.md`, pronto para substituir o arquivo em
`Joao-Pesquisa\_entregas\Relatorio_Cap17_Joao.md` na máquina do usuário.
Verificado por `grep` que só a ocorrência de 17.5 mudou — o `^HM^` de
17.22 (leituras patrísticas minoritárias sobre a glória) é rótulo correto
e ficou intacto. **A gravação final no arquivo de origem depende do
usuário salvar o arquivo entregue no lugar certo** — este repositório
segue sem acesso de escrita a ele.

**⚠️ Achado: rigor desigual entre as duas refutações da Regra Zero.** A
refutação de 17.20-21 (ecumenismo) enumera os cinco itens explicitamente
no corpo do texto — "(1) fonte primária... (2) melhor versão... (3) ataque
ao pressuposto... (4) ancoragem tripla... (5) desfecho". A refutação da
tese de Bultmann sobre 17.3 (mito do redentor gnóstico) é substantiva e
bem ancorada (Colpe, Schenke, Brown, Hengel, Frey), mas **não percorre os
cinco itens de forma explícita** — não há passagem que nomeie o
pressuposto de Bultmann como tal, nem um desfecho formalmente marcado.
Mesmo padrão vale para a refutação das heterodoxias de 17.5: substantiva,
mas sem a numeração explícita. Isto não é necessariamente falha — o
padrão de cinco itens exige que os cinco **estejam presentes**, não que
sejam rotulados — mas a inconsistência de forma entre as três refutações
do mesmo relatório é o tipo de coisa que vale nivelar numa revisão.

✅ **Reformatado em 28/09/2026, a pedido do usuário** — as duas
refutações (17.5 e Bultmann/17.3) foram reescritas no mesmo molde
explícito de (1)-(5), usando **só o conteúdo já presente no relatório**,
sem acrescentar citação ou argumento novo. Entregue como parte do
`Relatorio_Cap17_Joao_CORRIGIDO.md` (v2).

⚠️ **A reformatação não foi cosmética — expôs lacuna de conteúdo real,
não só de forma**, exatamente o risco que se previa ao tentar nivelar o
rigor sem inventar. Em ambas as refutações, dois dos cinco itens ficaram
com nota de auditoria em vez de conteúdo, porque o texto original não o
tinha:

| Item | 17.5 (heterodoxias) | Bultmann (17.3) |
|---|---|---|
| (1) fonte primária | descreve as três posições, **não nomeia autor/obra** de nenhuma | nomeia Bultmann e a obra, mas **sem página** conferida |
| (4) recepção patrística + consenso conservador | **ausente** — só ancoragem textual (item 4-texto) está de fato presente | idem — só ancoragem textual está presente |

Isto é diferente da refutação ecumênica (17.20-21), que tem os cinco
itens **com conteúdo real** em todos, não só com rótulo. A assimetria
original não era só de apresentação: as duas refutações mais fracas
**também têm menos substância** nos itens 1 e 4. Corrigir isso de
verdade — nomear a fonte primária de cada heterodoxia, achar a página de
Bultmann, trazer a recepção patrística e o consenso conservador por nome
— exige consultar o corpus real (NotebookLM, `575759eb`), o que este
repositório não pode fazer. **A reformatação entregue é honesta sobre o
que ainda falta, não uma correção completa.**

✅ **Consulta ao corpus real feita em 28/09/2026 — o usuário rodou o
script no NotebookLM e trouxe as 4 respostas.** Depois de resolver 4
obstáculos técnicos em cadeia (pacote de cookies com nome trocado —
`rookiepy`, não `rookie-cookies`; certificado SSL interceptado por
antivírus/proxy, corrigido com `pip-system-certs`; conta errada logada no
Firefox; perfil ESR vs. normal), as 4 consultas rodaram contra o notebook
`575759eb`. Resultado, item por item:

- **Item 1 e 4 de 17.5 (heterodoxias): preenchidos com conteúdo real.**
  Achado relevante: **só a leitura unitária/sociniana tem fonte primária
  no dossiê** (`Spirit & Truth Fellowship International`, remetendo ao
  *Racovian Catechism*). Modalismo e arianismo **não têm** — e, no caso do
  arianismo, isso é em parte **perda histórica** (a *Thalia* de Ário foi
  destruída por decreto pós-Niceia), não só lacuna de aquisição. A
  ancoragem tripla (item 4) veio completa: quatro padres nomeados com obra
  e capítulo (Cirilo, Atanásio, Agostinho, Hilário) e sete comentaristas
  conservadores com página (Morris p.643, Ridderbos p.547, Carson p.554,
  Mounce p.358, Harris/Köstenberger p.70, Thompson p.422, Moloney p.172).
- **Item 1 de Bultmann (17.3): parcialmente preenchido.** O dossiê **não
  contém o comentário integral de Bultmann** — a consulta devolveu, com
  honestidade, "as fontes disponíveis não permitem afirmar isso com
  segurança" para a página exata. Isso vira pendência de aquisição
  explícita no relatório, não afirmação inventada.
- **Item 4 de Bultmann (17.3): ✅ preenchido em 28/09, na segunda
  rodada** (com o script de retry). Achado honesto e específico:
  **nenhuma fonte patrística no dossiê aplica a filologia de *yada'* a
  17.3** nem refuta Bultmann nominalmente — ausência declarada, distinta
  da recepção patrística geral do capítulo (que existe, mas para outros
  pontos). O consenso conservador veio com página, mas **fragmentado**:
  só Carson (edição em português, Vida Nova, pp. 557-558 e p. 27) e,
  parcialmente, Morris (p. 138 n. 191) combinam as duas pontas do
  argumento (matriz veterotestamentária + refutação nominal de
  Bultmann) no mesmo lugar; Ridderbos, Harris/Köstenberger e Rainbow
  sustentam uma ponta cada, não as duas.

**As três refutações do relatório agora têm os cinco itens preenchidos
— com conteúdo real do dossiê, ou com ausência explicitamente declarada
onde o dossiê de fato não tem a fonte.** Entregue como v4.

⚠️ **Ressalva que se aplica às páginas citadas em ambos os itens 4:**
vieram da resposta do NotebookLM sobre o dossiê, **não foram conferidas
contra o PDF original por este repositório** (que não tem acesso a
`biblioteca/`). Isso é exatamente o que a Regra 11 do projeto-mãe exige
antes de publicar como fato — "RAG para descobrir, disco para conferir".
Marcado no relatório como pendência explícita, não escondido.

**Entregue como v4** (`Relatorio_Cap17_Joao_CORRIGIDO.md`), via
`SendUserFile`. Pendências que sobram, todas fora do alcance deste
repositório: (a) **rodar `conferir_citacoes_cap17_item4.ps1`** para
confirmar em disco (`_processados_md\`) as páginas citadas por Carson,
Morris, Ridderbos, Mounce, Harris/Köstenberger, Thompson, Moloney, e as
referências de Cirilo/Atanásio/Agostinho/Hilário por numeração clássica
— entregue, ainda não executado; (b) decidir se adquire o comentário
integral de Bultmann para fechar o item 1 daquela refutação por
completo, hoje só descrito por fonte secundária.

**✅ Confirma, em vez de contradizer, os candidatos a expansão já
propostos em §1.3:** o gênero testamentário é tratado em termos gerais
("Testamento de Despedida"; Gn 49; Dt 31-33; *Testamento dos XII
Patriarcas*) sem citar nominalmente Segovia, Kurz ou qualquer monografia
dedicada ao gênero — e o próprio relatório declara em aberto o "pano de
fundo cultual (Yom Kipur vs. Qumran)" na síntese final. Os dois pontos já
apontados na v1 (§5.4 antiga; frente "gênero literário" em §1.3)
continuam sendo lacuna real, não presunção — o relatório confirma,
não invalida.

**Não verificável a partir daqui:** conferência de citação-por-citação
(`conferir_citacoes.py`) exige o PDF original de cada fonte (Carson,
Ridderbos, Cirilo etc.) para checar página e forma exata — este
repositório não tem acesso a `biblioteca/`. O mesmo vale para as 25
fontes "sem status" da poda de 21/09 (não estão listadas no relatório).
Estes dois itens de §1.1 continuam pendentes de execução no ambiente do
projeto-mãe.

**Nota lateral, sem ação:** o relatório (datado 11/09) descreve o corpus
como 337→316 fontes após poda mecânica. O `MEMORIA_PROJETO.md` (21-23/09)
registra um estado posterior — poda semântica 300→176. Não é
contradição: são medições em datas diferentes, a mais recente
prevalecendo para qualquer citação de "tamanho do corpus atual".

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
- **A Sentinela 17-A** (P66/P75 não cobrem Jo 17) — proposta na v1, **agora
  verificada contra o texto entregue: sem violação** (ver §1.1-B).

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
| 3 | ✅ **Feito em 28/09** — `Relatorio_Cap17_Joao.md` lido na íntegra; achados em §1.1-B. `conferir_citacoes.py` propriamente dito (página exata em cada PDF) segue pendente — exige `biblioteca/` | resultado parcial obtido; conferência fina depende do ambiente do projeto-mãe |
| 4 | ✅ **Feito em 28/09** — Sentinela 17-A verificada: sem violação (§1.1-B) | — |
| 5 | Levar ao usuário os dois achados de §1.1-B (rótulo `^HP^`/`^HR^` em 17.5; assimetria de rigor entre as três refutações) para correção no relatório do projeto-mãe | resposta do usuário |
| 6 | A partir da auditoria, decidir com o usuário **quais das frentes de expansão (§1.3, e a nova frente de crítica textual do capítulo aberta em §1.1-B)** valem o investimento de uma obra dedicada, e em que ordem | resultado de 1-5 |

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

---

## 5. Conferência local (Regra 11) — resultado da primeira rodada, 28/09/2026

O script v1 (`conferir_citacoes_cap17_item4.ps1`) rodou contra
`_processados_md\`, buscando as frases da resposta do NotebookLM
**traduzidas para português** — defeito de desenho meu: os PDFs de
origem (Morris, Ridderbos, Carson-inglês, Harris/Köstenberger, Thompson,
Moloney) são majoritariamente em **inglês**; buscar "clara" ou "glória"
onde o texto diz "clear" ou "glory" falha sempre, **não** porque a
citação seja falsa. Resultado: 8 de 10 citações "não encontradas" — por
esse motivo, não por refutação real. Mounce e Hilário: arquivo não achado
(pode ser real ausência do corpus, ou nome de arquivo diferente —
verificar na lista completa que o v2 gera).

**As 5 ocorrências "encontradas" de Agostinho eram todas falsos
positivos, confirmado por leitura direta:**
- `Agostinho_ATrindade.md` (5x): "105" é número de página, nota de
  rodapé e versículo — nunca "Tratado 105". E é *De Trinitate*, obra
  errada (não é a coleção de *Tractates on John*).
- `Agostinho_Tractates_NPNF107_COMPLETO.md` (31x): mesmo padrão — página,
  nota, número de salmo, índice do fim do livro. O trecho que a busca
  trouxe é do capítulo 12 de João, não do 17.
- `Agostinho_Homilias_Joao_1-40_Hill.md` (9x): **estruturalmente
  impossível conter o Tratado 105** — o nome do arquivo já diz que essa
  edição cobre só os Tratados 1-40.
- `Agostinho_Tractates_NPNF107_P1de2.md` (25x): a coleção completa tem
  124 tratados; dividida ao meio, a primeira parte cobre por volta de
  1-62 — o Tratado 105 deveria estar na segunda metade (`P2de2`).

**Conclusão:** a citação "Agostinho, *Tratados sobre o Evangelho de
João*, Tratado 105.5-8" — usada no item 4 da refutação de heterodoxias de
17.5 — **continua não verificada**, nem confirmada nem refutada. A busca
de v1 nunca chegou perto do lugar certo.

**Corrigido no v2** (`extrair_paginas_cap17_v2.ps1`, já entregue): em vez
de buscar frase traduzida, extrai o texto ao redor do **marcador de
página real** mais próximo do número alegado (com janela ampliada para
cobrir o deslocamento conhecido, `CLAUDE.md` P-04), e lista todos os
arquivos de `_processados_md\` para resolver Mounce/Hilário. Ainda não
rodado pelo usuário. Para Agostinho especificamente, a busca certa não é
por número de tratado solto — é por conteúdo do capítulo 17 (a coleção
completa organiza por capítulos do Evangelho, não por número de tratado,
como ficou visível nos trechos extraídos) — ajuste a fazer se o v2 também
não achar.

**Achado de 28-29/09/2026, rodando o v2: `Carson_Joao.md` tem três
defeitos distintos, não um.** O v2 reportou "sem marcadores de página
reconhecíveis" para os 6 arquivos-alvo (Morris, Ridderbos, Carson,
Harris_EGGNT, Thompson, Moloney). Inspeção direta de `Carson_Joao.md`
revelou por quê:

1. **Marcador existe, mas corrompido por codificação dupla de UTF-8** —
   o arquivo tem `<!-- PÃ¡gina 1 -->` em vez de `<!-- Página 1 -->`
   (mojibake: bytes UTF-8 de "á" lidos como Latin-1/CP1252 e regravados).
   O mesmo defeito aparece no frontmatter (`tÃ­tulo`, `JOÃƒO`) — não é
   artefato de exibição do console (outros arquivos, como os de
   Agostinho, mostraram acentuação correta na mesma sessão), é corrupção
   real do arquivo em disco.
2. **Página 1 tem OCR ilegível** — `1 = oA . Se cao E Ego & Pa...` — não
   é o aviso de grego já registrado no cabeçalho do arquivo (que fala só
   de grego); é falha de reconhecimento geral. Ainda não verificado se
   isso afeta só a primeira página ou o documento inteiro, incluindo as
   páginas 554 e 27 usadas nas citações do relatório.
3. **Intercalação de nota de rodapé** (já registrado acima) — mesmo
   arquivo, defeito adicional e independente.

**Decisão do usuário (28/09):** reconverter `Carson_Joao.md` com
`_scripts\pdftotext_para_md.py` — a ferramenta que o próprio
`CLAUDE.md`/`MEMORIA_PROJETO.md` já documenta como correção para a
intercalação de nota (Regra 11-B), e que provavelmente também resolve a
codificação dupla, por usar `pdftotext` em vez do PyMuPDF problemático.
**Aguardando a sintaxe exata do script** (pedido ao usuário: mostrar as
primeiras 30 linhas) antes de indicar o comando de reconversão. Até lá,
as citações de Carson (pp. 554, 27, 557-558) permanecem **não
verificadas**, e a mesma suspeita de codificação dupla precisa ser
checada nos outros 5 arquivos-alvo antes de tentar de novo a extração por
marcador.

## 6. Reconversão e conferência de Carson — concluída em 29-30/09/2026

A sintaxe real do script era `pdftotext_para_md.py pdf saida --titulo
TITULO --autor AUTOR` (dois posicionais + duas flags obrigatórias que eu
não previ nas quatro tentativas automáticas). O PDF certo também exigiu
correção: a primeira busca automática achou por engano *Father, Son and
Spirit* (Köstenberger, Swain **e** Carson) em vez do comentário solo de
Carson sobre João — mesmo tipo de erro de casamento por nome que o
projeto-mãe já documentou (Regra 12). Reconvertido com sucesso: 687
páginas, 364.667 palavras.

**Resultado da conferência real, por leitura direta do texto (não mais
busca de string):**

| Citação | Resultado |
|---|---|
| Carson, pp. 557-558 (matriz veterotestamentária de "conhecer", item 4 de Bultmann/17.3) | ✅ **Confirmado ao pé da letra** — Jr 31.34, Os 4.6, Hc 2.14, Pv 3.6, Dt 30.20 aparecem literalmente |
| Carson, p. 27 ("refutação do mito gnóstico de Bultmann") | ❌ **Não confirmado como caracterizado** — pp. 26-28 são exposição histórico-descritiva do gnosticismo antigo (Valentino, Herácleo), não uma refutação argumentada da cronologia de Bultmann. Pode existir em página não coberta pela janela lida |
| Carson, p. 554 ("sintaxe de *para* + dativo", item 4 de 17.5) | ❌ **Não confirmado nesta página** — p. 554 trata da estrutura do capítulo, não da sintaxe do v. 5. A exegese real do v. 5 está na p. 558, que afirma a pré-existência real (tese correta) mas **sem o argumento gramatical específico** que a citação atribuía a Carson nessa página |

**Consequência para o relatório:** reescrevi os dois trechos (v5,
entregue) para refletir isso com precisão — mantendo o que é verdadeiro
(Carson afirma pré-existência real em 17.5; a matriz veterotestamentária
em Bultmann/17.3 está confirmada) e marcando honestamente o que não se
sustenta como antes descrito, em vez de manter uma citação de página
errada.

**O que isso ensina sobre o método:** de três citações de Carson
verificadas por leitura direta, **uma bateu exatamente, uma bateu
tematicamente mas não no ponto técnico, e uma não bateu de jeito
nenhum.** Confirma exatamente o motivo pelo qual o projeto exige "RAG
para descobrir, disco para conferir" — a resposta do NotebookLM sobre o
dossiê é plausível o bastante para não ser questionada sem essa
conferência, e ainda assim erra 2 de 3 vezes neste caso.

**Pendência que resta:** os outros 6 autores citados no item 4 (Morris,
Ridderbos, Mounce, Harris/Köstenberger, Thompson, Moloney) — e os 4
patrísticos (Cirilo, Atanásio, Agostinho, Hilário) — continuam **sem
conferência em disco**, pelo mesmo motivo original (arquivos sem
marcador de página reconhecível, possivelmente pelo mesmo defeito de
codificação dupla que afetava Carson). Reconvertê-los um a um segue o
mesmo roteiro que resolveu Carson.

## 7. Morris e Ridderbos conferidos — 30/09/2026: o achado mais sério até aqui

Reconvertidos com a mesma sintaxe (um bug próprio corrigido no meio do
caminho: a função do script capturava a saída do `python` junto com o
caminho do arquivo via `Tee-Object`, poluindo o retorno — corrigido
rodando a extração à parte). Resultado da conferência por leitura direta
de 5 citações (Morris ×2, Ridderbos ×3):

| Citação | Resultado |
|---|---|
| Morris, p. 643 (17.5, pré-existência) | ✅ **Confirmado quase ao pé da letra** — "There is a clear assertion of Christ's pre-existence here..." |
| Morris, p. 138 n. 191 (Bultmann/Nag Hammadi) | ❌ **Não confirmado, página inteiramente errada** — conteúdo real é sobre João Batista/Elias, nada de Bultmann |
| Ridderbos, p. 547 (17.5, glória preexistente) | ❌ **Não confirmado, capítulo errado** — a página é exegese de João 15, não 17 |
| Ridderbos, pp. 12-14 (Bultmann) | ⚠️ **Mal caracterizado, quase o oposto** — Bultmann é citado como modelo metodológico que Ridderbos segue, não como alvo de refutação |
| Ridderbos, p. 95 (Bultmann) | ❌ **Não confirmado** — conteúdo é sobre João 1 (João Batista), sem relação com Bultmann |

**Taxa agregada até agora, contando também as 3 de Carson: 3 confirmadas
de 8 checadas — pouco mais de 1 em 3.** Isso muda o peso que qualquer
citação de página **desta lista de fontes ainda não conferida** deveria
receber — Mounce, Harris/Köstenberger (nos dois pontos em que aparece),
Thompson, Moloney e Rainbow precisam ser tratados como **não
verificados**, não como fato, até passarem pelo mesmo processo.

Reescrevi os dois blocos do relatório (v6, entregue) refletindo isso —
inclusive nomeando explicitamente a taxa de acerto agregada como razão
para desconfiar do que ainda não foi conferido, em vez de deixar a
impressão de que só as fontes já checadas importam.

**Padrão que emerge, útil para o resto da conferência:** os erros não
são aleatórios — nos três casos "não confirmados", a página citada tem
conteúdo de **outro capítulo do livro inteiro** (João 1 ou João 15, não
João 17), o que sugere que o RAG às vezes cita a página certa **de um
tema relacionado tratado em outro lugar do mesmo livro**, não uma
invenção pura. Vale, ao conferir os próximos, checar também ±0-2
capítulos de distância antes de declarar "não encontrado" de vez.

## 8. Cópia completa do projeto-mãe — 30/09/2026

A pedido do usuário, todo o `Joao-Pesquisa` foi copiado para
`C:\Users\admintrt9a\Projetos\JOAO17`, via `robocopy` (script único que
checa espaço, fecha o Firefox — não mata `python*`, por causa do alerta
já registrado no próprio `MEMORIA_PROJETO.md` contra encerrar processo
por regex —, copia, e confere por tamanho e contagem de arquivos, não só
pelo código de saída do robocopy). **Verificado: 2.647 arquivos, 4,82
GB, origem e destino idênticos.** A partir de agora, `Projetos\JOAO17` é
uma cópia local completa e íntegra, independente de `Documents\
Joao-Pesquisa` — útil como backup e como espaço de trabalho isolado para
o aprofundamento de Jo 17 sem risco de interferir no projeto-mãe em
andamento.
