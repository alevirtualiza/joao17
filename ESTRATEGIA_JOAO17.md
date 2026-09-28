# Estratégia — Pesquisa Ampla, Profunda e Detalhada sobre João 17

*Elaborado em 28/09/2026, a partir dos quatro artefatos do projeto-mãe
(`CLAUDE.md`, `CHECKPOINT_PROJETO.md`, `AQUISICOES_ESCOLAS.md`,
`AQUISICOES_LACUNAS.md`). Este repositório (`joao17`) recorta do projeto
"Joao-Pesquisa" **um único capítulo** — a Oração Sacerdotal — e aplica a ele,
sem diluição, toda a metodologia já validada e testada em 46 erros e 30 lições
registrados no diário técnico do projeto-mãe. Não se reinventa método aqui;
herda-se o que já funcionou e se recorta o que é específico de Jo 17.*

---

## 1. Por que João 17 pede um projeto à parte, e não um capítulo entre 21

O projeto-mãe já classificou a Fase 2 (exegese por perícope) como não
iniciada — 21 capítulos, moldes prontos, zero execuções. João 17 tem motivo
para furar a fila:

1. **É o único capítulo do Evangelho que é, ele mesmo, uma unidade de gênero
   fechada** — oração, não narrativa nem discurso dialogado. Isso muda o
   método de leitura: precisa de literatura sobre **gênero de oração
   sacerdotal / testamentária**, que os demais capítulos não pedem.
2. **É o ponto de maior tráfego doutrinário do Evangelho.** Cristologia da
   glória (17.1-5, 24), Trindade e reciprocidade Pai-Filho, eleição e
   perseverança dos santos (17.2, 6, 9, 12), definição de vida eterna (17.3),
   consagração pela verdade (17.17), missão (17.18), e a unidade dos crentes
   (17.20-23) — este último o texto mais citado do Evangelho em debates
   ecumênicos contemporâneos, dentro e fora do campo confessional que o
   projeto-mãe adota.
3. **O corpus já tem mais fonte dedicada a Jo 17 do que a quase qualquer outro
   capítulo isolado** — Lloyd-Jones escreveu exposição exclusiva sobre ele, e
   isso já está no acervo. É o capítulo onde menos se depende de aquisição
   nova e mais se depende de leitura cuidadosa do que já se tem.
4. **A Regra Zero (§0 do `CLAUDE.md`) tem aqui seu teste mais difícil.** A
   leitura ecumênica/católica de 17.21-23 ("para que todos sejam um... para
   que o mundo creia") é historicamente usada como base para eclesiologia de
   unidade visível institucional — divergente da leitura evangélica-reformada
   de unidade espiritual invisível. É o lugar do Evangelho onde a linha
   editorial do projeto mais precisa de disciplina para não decretar a
   refutação em vez de argumentá-la.

---

## 2. Recorte textual e estrutura literária — a base de tudo o que segue

João 17.1-26 divide-se, por consenso quase unânime da literatura (Calvino,
Ridderbos, Bernard, Carson, Köstenberger, Barrett, Brown), em **três
movimentos concêntricos**, não em versículos soltos. A exegese deve respeitar
essa arquitetura — é o que evita o erro mais comum do gênero (comentário
versículo a versículo que perde o arco):

| Bloco | Versículos | Conteúdo | Categoria teológica dominante |
|---|---|---|---|
| **I — Jesus ora por si mesmo** | 17.1-5 | Pedido de glorificação mútua; vida eterna definida (17.3); glória pré-encarnação (17.5) | Cristologia, glória, pré-existência |
| **II — Jesus ora pelos discípulos presentes** | 17.6-19 | Guarda (17.11-12, Judas), separação do mundo, santificação pela verdade (17.17), envio em missão (17.18) | Eclesiologia, perseverança, santificação |
| **III — Jesus ora pelos crentes futuros** | 17.20-26 | Unidade dos crentes (17.20-23), visão da glória (17.24), conhecimento do Pai e amor (17.25-26) | Unidade da igreja, escatologia, Trindade |

**Consequência metodológica:** o capítulo não comporta um único prompt
exegético. Segue-se o padrão de **três sub-notebooks de trabalho ou três
blocos de prompt** dentro de um único notebook NotebookLM — um por bloco —,
preservando o limite de 4-5 prompts exegéticos por sessão (`CLAUDE.md` §3,
ajustado para 5 em 09/08/2026) sem forçar leitura rasa de um capítulo com
peso desproporcional ao número de versículos.

---

## 3. Metodologia herdada — aplicada linha a linha

Nada abaixo é novo; é a tradução do que já está em `CLAUDE.md` §2-B, §3, §4
para o caso concreto de Jo 17.

### 3.1 Regra Zero aplicada a Jo 17

A objeção progressista mais forte especificamente sobre este capítulo não é
histórico-crítica clássica, é **eclesiológica-ecumênica**: a leitura de
17.21-23 como mandato para união institucional visível das igrejas (linha
católico-romana pós-Vaticano II e do Conselho Mundial de Igrejas), contra a
leitura reformada-evangélica de unidade essencialmente espiritual, manifesta
mas não dependente de estrutura institucional única. A Regra Zero exige que
esta seja tratada como objeção a refutar — na sua melhor forma — não como
duas leituras igualmente válidas. Ver §5.2 abaixo para as fontes primárias
necessárias dos dois lados.

Uma segunda linha de tensão, interna ao campo conservador e não externa a
ele, é **calvinista × arminiana/wesleyana** sobre 17.9 ("não rogo pelo mundo")
e 17.12 (segurança dos guardados, "nenhum se perdeu, senão o filho da
perdição") — eleição/perseverança versus livre-arbítrio e possibilidade de
apostasia. Aqui a Regra Zero **não se aplica da mesma forma**: são duas
posições dentro do espectro confessional que o projeto já tem instrução para
tratar por escola (§4 abaixo), não uma objeção liberal a decretar vencida.
Confundir os dois casos — tratar Wesley como "objeção liberal" — seria erro
de categoria, o mesmo tipo que o projeto-mãe já registrou ao arrolar Hengel
erroneamente entre defensores de uma tese que ele não sustenta.

### 3.2 O padrão de cinco itens, por objeção

Cada objeção que o capítulo abrir — ecumênica sobre 17.21-23, crítica sobre a
autenticidade histórica da oração (Bultmann: composição joanina tardia, não
palavras de Jesus), ou sobre o gênero (a oração como construção literária
helenística/testamentária e não relato) — precisa cumprir os cinco itens do
`CLAUDE.md` §2-B antes de fechar seção. Not cumprir os cinco = declarar a
lacuna, nunca decretar.

### 3.3 Sentinelas aplicáveis (das 9 do projeto-mãe)

Duas das nove sentinelas gerais tocam diretamente Jo 17 e precisam entrar no
checkpoint factual deste capítulo:

- **Egō eimi** — 17.3 não usa a fórmula absoluta, mas a definição de vida
  eterna ("conhecer... a ti, único Deus verdadeiro, e a Jesus Cristo") é o
  ponto onde a cristologia joanina da identidade divina de Jesus se articula
  com mais densidade doutrinária fora das fórmulas *egō eimi* propriamente
  ditas — merece nota own, não fusão com a sentinela existente.
- **Testemunhos textuais (P66, P75, ℵ, B, D)** — conferir cobertura: P66
  cobre até 14.26, portanto **não cobre Jo 17**; P75 cobre até 15.8,
  **também não cobre Jo 17** integralmente. Isso é factualmente relevante e
  costuma ser omitido: a crítica textual de Jo 17 depende de outros
  manuscritos (ℵ, B, e os unciais posteriores), o que enfraquece qualquer
  alegação de suporte papiráceo antigo direto para este capítulo
  especificamente. **Verificar isso em Metzger/NA28 antes de escrever
  qualquer afirmação sobre o texto de Jo 17 — não presumir a partir da
  cobertura geral de P66/P75.**

Propõe-se registrar isso como **Sentinela 17-A** (específica deste projeto,
não do projeto-mãe): *"Jo 17 está fora do alcance de P66 e P75. Nunca citar
esses papiros para estabelecer o texto de Jo 17 especificamente."*

### 3.4 As três consultas por bloco (não por capítulo inteiro)

Adaptação necessária do protocolo padrão (`CLAUDE.md` §2-B): como o capítulo
tem três blocos teologicamente distintos, a consulta de verificação
("quem, no dossiê, sustenta o contrário?") deve ser **disparada por bloco**,
não uma vez para o capítulo inteiro — um único disparo geral tenderia a
recuperar só a objeção mais saliente (a ecumênica) e teria retrieval fraco
sobre as objeções mais técnicas de 17.1-5 (pré-existência) e 17.6-19
(perseverança).

---

## 4. O que o corpus já tem para Jo 17 — auditoria por escola

*Baseado no que `AQUISICOES_ESCOLAS.md` e `CLAUDE.md` §2-B já registram
como estado do corpus em 28/07 e 01/08/2026. Antes de qualquer aquisição
nova, ler esta tabela — é a aplicação da Regra 11 do projeto-mãe ("RAG para
descobrir, disco para conferir") ao próprio planejamento.*

| Escola | Fonte já no corpus, e o que ela cobre em Jo 17 | Estado |
|---|---|---|
| **Reformada** | **Lloyd-Jones** — exposição **dedicada** a Jo 17, já citada nominalmente em `AQUISICOES_ESCOLAS.md` linha 133 como a referência reformada do capítulo. Calvino (3 vols.), Ridderbos, Matthew Henry, Bernard (ICC) — todos cobrem o Evangelho inteiro, logo cobrem 17 | 🟢 forte |
| **Patrística** | Crisóstomo (88 homilias, extraído — cobre 17 dentro do intervalo geral), Cirilo de Alexandria (2 vols.), Agostinho (Homilias sobre João, Hill e NPNF), Von Wahlde vol. 3 (caps. 13-21, portanto Jo 17 integralmente) | 🟢 forte, mas conferir se Crisóstomo/Cirilo de fato **comentam** 17 e não apenas o cercam — aplicar a mesma checagem que o projeto-mãe já fez com Bengel/Wesley em autoria (presença ≠ cobertura do tema) |
| **Católica/moderna** | **Schnackenburg vol. 3** (*ai capp. 13-21*, edição italiana Paideia, já adquirida e amostrada — a amostra confirmada em `AQUISICOES_LACUNAS.md` linha 99 discute **exatamente 17.20-23**, a unidade dos crentes) | 🟢 **peça central para a objeção ecumênica** — já no acervo |
| **Puritana** | Hutcheson (*Exposition*, integral, versículo a versículo) | 🟢 se adquirida (ver §5.3) |
| **Pietista** | Bengel (*Gnomon*, João extraído p. 332-451 — conferir se o recorte inclui 17) | 🟡 conferir cobertura real |
| **Wesleyana** | Wesley (*Explanatory Notes*, João extraído p. 226-294 — conferir cobertura de 17), Adam Clarke vol. 5B (integral, cobre 17) | 🟢 Clarke; 🟡 conferir Wesley |
| **Pentecostal** | Keener (*The Spirit in the Gospels and Acts*) — Jo 17 não é o foco natural desta obra (o Paráclito está em 14-16), mas 17.17-19 (santificação, missão, envio) é ponto de contato pneumatológico possível | 🟡 conferir se o livro chega a tratar 17 ou se é preciso **declarar o silêncio** |
| **Crítica/histórica** | Bultmann (já no corpus, 3 contagens de palavra registradas) — fonte primária da tese de composição tardia/não-histórica da oração | 🟢 necessário para cumprir item 1 do padrão de refutação sobre a objeção histórico-crítica |

**Ação imediata, antes de qualquer Deep Research:** rodar em cada uma das
fontes marcadas 🟡 uma consulta de localização simples — "o que esta obra diz
sobre Jo 17?" — e registrar se a resposta é substantiva ou silenciosa. É o
mesmo procedimento que o projeto-mãe já aplicou a Bengel e Wesley em autoria,
e que já provou pegar presença sem cobertura.

---

## 5. Lacunas específicas de Jo 17 — o que falta e por quê

### 5.1 Já resolvido no projeto-mãe, herdado de graça

**Schnackenburg vol. 3** — a maior lacuna católica que o projeto-mãe
registrou (`AQUISICOES_LACUNAS.md` §4) foi suprida pela edição italiana da
Paideia, e a amostra de verificação **é justamente o trecho de 17.20-23**.
Isto é: a obra mais crítica para o bloco III deste capítulo específico já
está confirmada em mãos, com uma ressalva técnica herdada — o grego sai como
sósia latino (fonte Type1 sem ToUnicode) e **não deve ser citado em forma
grega acentuada a partir deste PDF**; para grego usar Harris (EGGNT) ou
Barrett, também já no acervo.

### 5.2 A lacuna ecumênica — a mais urgente deste projeto, específica dele

Nem `AQUISICOES_ESCOLAS.md` nem `AQUISICOES_LACUNAS.md` — escritos para o
projeto inteiro — trazem fonte primária **do lado ecumênico/católico
contemporâneo** que defenda a leitura institucional de 17.21-23. Isto é uma
lacuna que só aparece ao recortar Jo 17 isoladamente; no projeto-mãe ela
estava invisível, diluída entre 21 capítulos.

Sem essa fonte, a Regra Zero e o item 1 do padrão de cinco itens (fonte
primária localizável) **não podem ser cumpridos** para esta objeção
específica — o capítulo teria de declarar a lacuna em vez de refutar, o que
seria uma perda séria, dado que 17.20-23 é o texto mais citado do Evangelho
em discurso ecumênico público.

**Candidatos a levantar (dados de conhecimento do redator, não do
corpus — conferir na aquisição, seguindo a mesma advertência que
`AQUISICOES_LACUNAS.md` já impõe a si mesma):**

| Obra | Autor | Papel |
|---|---|---|
| *Unitatis Redintegratio* (decreto conciliar, 1964) + comentário católico padrão | Concílio Vaticano II | fonte primária do magistério católico sobre unidade visível, citando diretamente Jo 17 |
| *That They May Be One: A Study of Papal Doctrine* ou equivalente | a conferir | leitura católica confessional de Jo 17.21 |
| Documentos do Conselho Mundial de Igrejas sobre unidade visível | WCC/Faith and Order | a versão ecumênica protestante-liberal, distinta da católica |
| Resposta evangélica-reformada dedicada | candidatos: D. A. Carson (*The Farewell Discourse*), Köstenberger, ou o próprio Lloyd-Jones já no acervo | a réplica confessional — conferir se já cobre isso antes de comprar mais |

**Nota de método:** esta é exatamente a situação que `AQUISICOES_LACUNAS.md`
resolveu para o Bloco A (Gardner-Smith) — procurar primeiro em disco (Regra
"nenhum índice prova ausência fora do próprio escopo") antes de declarar
ausência e sair à cata. É possível que Carson ou Köstenberger, já
mencionados no corpus geral do projeto-mãe, tratem disso — **conferir antes
de comprar**.

### 5.3 Lacunas herdadas, ainda não fechadas, que tocam Jo 17

Da tabela de "Quadro de decisão" de `AQUISICOES_LACUNAS.md`:

- **Neirynck** e **Jaubert** — lacunas declaradas, decisão do usuário de
  seguir sem elas. Não tocam Jo 17 diretamente (sinóticos e cronologia da
  paixão) — **fora do escopo deste projeto**, não repetir a tentativa aqui.
- **Hoehner** — cronologia da vida de Cristo; toca Jo 17 apenas
  perifericamente (datação da Última Ceia, contexto da oração). Prioridade
  baixa para este projeto especificamente.
- **Hutcheson** (puritano) — se ainda não convertido/subido ao notebook
  geral, verificar estado antes de assumir cobertura na tabela do §4 acima.

### 5.4 Gênero literário — a oração sacerdotal como testamento

O projeto-mãe já identificou, para o cap. 6 (discurso de despedida, Jo 14-16),
a lacuna de **Segovia** (*The Farewell of the Word*) e **Kurz** (*Farewell
Addresses in the New Testament*, tratando do gênero testamentário judaico).
Jo 17 é a **conclusão** do discurso de despedida e compartilha o mesmo
problema de gênero — na verdade, a oração sacerdotal é justamente o ponto
onde o gênero "testamento" se completa com uma oração de intercessão, paralela
a Moisés (Dt 32-33), aos testamentos dos patriarcas intertestamentários, e à
liturgia sacerdotal judaica (Yom Kipur). **Esta é uma lacuna que Jo 17 herda
do cap. 6 e agrava**: nenhuma das duas obras (Segovia, Kurz) é dedicada à
oração especificamente. Considerar, adicionalmente:

| Obra | Papel |
|---|---|
| David Aune ou similar sobre gênero de oração antiga | pano de fundo greco-romano e judaico de oração solene |
| Literatura sobre *Yom Kipur* e o sumo sacerdote (origem do nome tradicional "Oração Sacerdotal", cunhado por David Chytraeus no séc. XVI, não pelo texto) | conferir se o corpus tem algo sobre a tipologia sacerdotal levítica aplicada a Jo 17 — provável **lacuna a declarar**, não presumir |

---

## 6. Plano de execução

### 6.1 Notebook dedicado

Criar `Joao - Cap 17 - Oracao Sacerdotal`, seguindo `montar_notebook_capitulo.ps1`
do projeto-mãe (herdado, não reescrito). Corpus base: todas as fontes do §4
marcadas 🟢, mais os candidatos do §5.2 assim que adquiridos. Meta: ~55 fontes
de corpus + Deep Research dirigida (Pro: até 300/notebook, mas a curadoria
R1-R4 do `_triagem_dr/` do projeto-mãe deve ser aplicada integralmente —
nenhuma DR entra sem triagem).

### 6.2 Sequência de prompts exegéticos (respeitando o limite de 5/sessão)

| Sessão | Bloco | Prompts |
|---|---|---|
| 1 | Bloco I (17.1-5) | (a) exegética — glória, vida eterna, pré-existência; (b) verificação — quem discorda da leitura de pré-existência real em 17.5; (c) refutação dirigida se a verificação abrir objeção |
| 2 | Bloco II (17.6-19) | (a) exegética — guarda dos discípulos, Judas, santificação, missão; (b) verificação — tensão calvinista/arminiana sobre 17.9, 12; (c) refutação/exposição das duas leituras confessionais **sem Regra Zero** (é debate intra-conservador — ver §3.1) |
| 3 | Bloco III (17.20-26) | (a) exegética — unidade, glória futura, conhecimento e amor; (b) verificação — a leitura ecumênica/católica na sua melhor forma (depende de §5.2 resolvido); (c) refutação plena pelos cinco itens |
| 4 | Transversal | (a) checkpoint factual — sentinelas 17-A e egō eimi/vida eterna; (b) consulta sobre gênero (testamento/oração sacerdotal), declarando lacuna se §5.4 não resolvido |
| 5 | Síntese do capítulo | redação final, auditoria de citações, rótulos de certeza revisados |

### 6.3 Deep Research — pauta dirigida (antes de qualquer DR genérica)

Toda DR deste capítulo abre, como manda `CLAUDE.md` §2-B, com *"quais
objeções progressistas este texto atrai?"* — aqui, concretamente:

1. A leitura ecumênica institucional de 17.21-23, na sua melhor forma
   católica **e** na sua melhor forma conciliar-protestante (são duas, não
   uma — WCC e Roma divergem entre si também).
2. A tese crítica de que a oração é composição joanina tardia retroprojetada
   na boca de Jesus (Bultmann e herdeiros) — contra a historicidade da cena.
3. Leituras que dissolvem a pré-existência de 17.5 em categoria mítica ou
   poética, não metafísica real.

### 6.4 Auditoria antes de fechar

Aplicar integralmente a Definition of Done do projeto-mãe (`CHECKPOINT_PROJETO.md`
§8.1): estrutura tese→objeções→resposta, rótulos de certeza em toda
afirmação, consulta de verificação por bloco (não só por capítulo),
checkpoint factual com as sentinelas aplicáveis + Sentinela 17-A, nenhuma
atribuição de ocorrência única, citações conferidas.

---

## 7. Riscos específicos deste recorte

| Risco | Por que é específico de Jo 17 | Mitigação |
|---|---|---|
| **Decretar a refutação ecumênica em vez de argumentá-la**, por falta da fonte primária do lado institucional | É o texto mais carregado ideologicamente do Evangelho e o mais fácil de responder por decreto | Não escrever a seção antes de §5.2 resolvido; declarar lacuna se a aquisição não vier a tempo |
| **Confundir debate calvinista-arminiano com objeção liberal** (ver §3.1) | Jo 17.9-12 é terreno de disputa confessional interna, não externa | Tratar por escola (§4), não pela Regra Zero |
| **Citar P66/P75 para o texto de Jo 17** | erro fatual fácil de cometer por generalização da cobertura desses papiros no Evangelho todo | Sentinela 17-A |
| **Presumir cobertura de Bengel/Wesley/Keener em Jo 17 sem checagem** | o projeto-mãe já documentou esse erro exato para autoria (presença ≠ cobertura) | Consulta de localização simples em cada fonte 🟡 do §4, antes de redigir |
| **Fragmentar o capítulo em 26 versículos isolados**, perdendo a arquitetura dos três blocos concêntricos | é o erro mais comum do gênero comentário | Seguir §2 como espinha estrutural obrigatória do relatório final |

---

## 8. Entregável

`Relatorio_Cap17_Joao.md/.docx/.pdf` — estrutura: introdução ao gênero e
recorte (§2 e §5.4) → Bloco I → Bloco II → Bloco III → síntese teológica
(cristologia, eclesiologia, unidade) → apêndice de sentinelas e checkpoint
factual. Alimenta depois, sem decidir nada de novo, o notebook de síntese
geral do projeto-mãe (`CLAUDE.md` §1.2), onde a coerência com os capítulos 1
(prólogo — pré-existência), 6 (discurso de despedida — gênero) e 10
(cristologia geral) deve ser verificada por contradição, não reaberta.
