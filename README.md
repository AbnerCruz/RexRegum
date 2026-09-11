# Scriptura — v0.3

> Um estudo bíblico progressivo, investigável e centrado na própria Escritura.

## Manifesto

Scriptura é um **website de investigação bíblica**. Não é catálogo de links, feed de artigos, enciclopédia de opiniões nem interface de aplicativo disfarçada de site. O objetivo é permitir que o leitor examine o texto, as relações internas da Escritura e, quando uma afirmação for empiricamente verificável, a própria evidência relevante **sem abandonar a experiência de estudo**.

## Autoridade e método

Para doutrina, teologia e hermenêutica, o projeto trabalha em regime **sola Scriptura**: nenhuma conclusão é fundamentada em credo, concílio, denominação, comentarista, pai da igreja ou autoridade religiosa externa. A interpretação é construída com texto, contexto, gramática e relações internas da própria Escritura.

Fontes externas são admitidas somente para fatos externos e testáveis: manuscritos, inscrições, objetos, cronologia, geografia, história material, proveniência, datação e estado de conservação. Elas servem para **examinar o dado**, nunca para decidir doutrina.

A regra metodológica é simples: observar primeiro, inferir depois e concluir apenas até onde os dados permitem. O site distingue explicitamente o que uma evidência demonstra, o que apenas corrobora, o que permanece incerto e o que a evidência não pode demonstrar.

## Um estudo = um tema

Nenhum estudo divide sua unidade com outro tema. Blocos e fases agrupam estudos apenas para orientação e progressão.

A trilha v0.3 contém **1.118 estudos unitários publicados**, distribuídos em 36 blocos. Cada estudo possui rota própria e uma estrutura de investigação completa:

- pergunta nuclear;
- texto-base ou objeto de investigação;
- orientação de escopo;
- percurso passo a passo;
- pontos de observação;
- síntese de controle;
- limites explícitos da conclusão;
- relações internas com outros estudos;
- estudo anterior e seguinte;
- fontes materiais/textuais, quando aplicáveis;
- progresso local no dispositivo.

A estrutura não substitui a leitura bíblica por uma resposta pronta. Ela organiza a investigação para que o estudante possa conferir cada conclusão.

## Tudo investigável dentro do site

Uma referência nunca deve funcionar apenas como saída para outro website. Ao ser ativada, abre um painel contextual dentro do próprio Scriptura.

### Referências bíblicas

Fluxo obrigatório:

1. tradução;
2. botão **Ver original**;
3. original hebraico/aramaico ou grego;
4. botão **Estudar o original** no topo da seção original;
5. forma, lema, transliteração, morfologia, léxico auxiliar e contexto;
6. retorno ao estudo exatamente no ponto de origem.

O leitor bíblico interno cobre a trilha completa e permite navegar por livro e capítulo quando a referência é ampla.

### Evidência material e textual

Manuscritos, inscrições e artefatos entram por fichas internas que apresentam, quando disponível:

- identificação e custodiante;
- datação e proveniência;
- dado incorporado ao estudo;
- o que a evidência permite concluir;
- o que não permite concluir sozinha;
- regra de uso dentro do Scriptura;
- link oficial como **auditoria secundária**, não como conteúdo principal.

Uma fonte externa não recebe autoridade hermenêutica por estar em museu, universidade ou instituição acadêmica. Sua função é documentar o dado externo que ela custodia.

## UX é requisito funcional

UX design e UX experience são a principal restrição de produto. Uma funcionalidade correta que seja cansativa, confusa, escondida ou faça o leitor perder contexto é considerada incompleta.

A v0.3 implementa:

- navegação web por URL/hash e histórico do navegador;
- leitor de estudo em página, sem transformar o website em shell de aplicativo;
- referências abertas em painéis contextuais;
- pesquisa e filtros da trilha;
- progresso local sem conta;
- retomada da leitura;
- estudos relacionados;
- navegação anterior/próximo;
- profundidade progressiva: tradução → original → análise;
- layout responsivo e foco em leitura;
- estados de foco e `prefers-reduced-motion`;
- carregamento sob demanda de corpora pesados.

## Arquivos principais

- `index.html` — website e motor de leitura/investigação.
- `estudos.js` — currículo canônico dos 1.118 estudos, motor editorial declarativo e registro de fontes primárias/institucionais.
- `README.md` — este manifesto.
- `PLANEJAMENTO.md` — especificação da trilha, contrato editorial, UX e critérios de auditoria.

## Estado da versão

A **v0.3 é a primeira versão com a trilha integral executável**. Todos os 1.118 temas planejados possuem unidade de estudo navegável e investigável. O antigo catálogo de 357 relações messiânicas permanece disponível como módulo especializado.

“Completo” aqui significa que nenhuma entrada da trilha permanece apenas como título ou placeholder: todas possuem estrutura de estudo, percurso, observações, síntese, limites e relações. Isso não transforma o corpus em algo imutável; fontes, metadados, traduções, análise linguística e UX continuam sujeitos a auditoria e refinamento quando houver dados melhores.

O projeto não aceita doações. O painel de apoio direciona o leitor a organizações humanitárias e convida, quanto ao Scriptura, apenas ao compartilhamento do projeto.

> **Que a graça do Senhor Jesus seja com todos.** — Apocalipse 22:21
