# PLANEJAMENTO — Scriptura

Versão do plano: **v0.1**  
Alvo de publicação: **GitHub Pages**  
Natureza do produto: **website responsivo; PWA apenas como progressive enhancement futuro**

---

## 1. Norte do produto

Construir um estudo bíblico **extenso, cumulativo e exaustivo por temas**, começando nos fundamentos verificáveis e progredindo até o encerramento do cânon cristão em Apocalipse 22:21.

A experiência deve permitir a um leitor sem formação técnica iniciar o percurso sem pré-requisitos, mas deve crescer até um nível de investigação textual profundo. O projeto não será uma coleção de artigos independentes: será uma **trilha de aprendizagem encadeada**.

### Regra de autoridade

- Para **doutrina, teologia e interpretação**: a argumentação deve ser *sola Scriptura*. Toda conclusão precisa ser sustentada por passagens bíblicas, contexto e relações internas do próprio texto.
- Para **afirmações empiricamente verificáveis**: usar fontes primárias ou institucionais responsáveis pelo objeto/dado. Ex.: imagem do manuscrito, catálogo de museu, publicação de escavação, inscrição, base textual.
- Fontes externas podem estabelecer fatos históricos ou textuais; não recebem autoridade para definir o significado teológico da Escritura.

---

## 2. Contrato editorial obrigatório

Cada estudo futuro deve separar visualmente:

1. **Pergunta** — o que exatamente está sendo investigado?
2. **Texto-base** — quais passagens são necessárias antes de qualquer conclusão?
3. **Observação** — o que está literalmente presente no texto?
4. **Relações internas** — onde a própria Escritura retoma, cita, explica ou desenvolve o tema?
5. **Evidência externa**, se aplicável — objeto/fonte direta, nunca opinião como substituto da evidência.
6. **Inferência** — quais conclusões decorrem dos dados apresentados?
7. **Limites** — o que os dados não permitem afirmar?
8. **Conclusão provisória ou final** — formulada apenas após os passos anteriores.
9. **Próximo fundamento** — qual conceito o estudante agora está pronto para estudar?

### Linguagem

- não pressupor conhecimento de hebraico, grego, história antiga ou crítica textual;
- não infantilizar;
- introduzir termos técnicos uma vez, com definição curta e reutilizável;
- evitar tom de sermão quando a etapa é demonstrativa;
- distinguir explicitamente **texto**, **observação**, **inferência** e **conclusão**;
- evitar “é óbvio”, “todos sabem”, “estudiosos concordam” e equivalentes como argumento.

---

## 3. Arquitetura da trilha

A ordem abaixo é uma **arquitetura inicial**, não um índice congelado. A regra é dependência lógica: um módulo só deve exigir conhecimentos já apresentados.

### BLOCO A — Podemos confiar no objeto que estamos lendo?

**01. O que pode ser testado empiricamente?**  
Escopo da evidência; diferença entre comprovar, corroborar e inferir; fontes diretas; limites da arqueologia.

**02. Que texto da Bíblia chegou até nós?**  
Manuscritos, famílias de testemunhos, variantes, cópia manual, comparação textual, códices, Manuscritos do Mar Morto, testemunhos do NT.

**03. Tradução: o que muda quando mudamos de língua?**  
Texto-fonte, equivalência, ambiguidades, variantes que afetam tradução, limites das traduções.

**04. O que significa “cânon” neste projeto?**  
Primeiro descrever o conjunto de livros e como os próprios textos se relacionam; história externa pode ser documentada em seção separada, sem transformá-la em fundamento doutrinário.

### BLOCO B — Como ler antes de interpretar

**05. Contexto imediato e argumento.**  
Versículo, parágrafo, seção, livro.

**06. Gênero e forma literária.**  
Narrativa, lei, poesia, profecia, sabedoria, evangelho, carta, apocalíptica.

**07. Citação, alusão, eco e tipologia dentro da própria Bíblia.**

**08. Palavra original sem falácia lexical.**  
Lema, forma flexionada, semântica, sintaxe, frequência e contexto.

### BLOCO C — A narrativa bíblica

**09. Criação.**  
**10. Humanidade, queda e morte.**  
**11. Juízo e preservação.**  
**12. Abraão e promessa.**  
**13. Êxodo e redenção.**  
**14. Lei, aliança e santidade.**  
**15. Tabernáculo, sacerdócio e sacrifício.**  
**16. Terra, juízes e reino.**  
**17. Davi, trono e promessa.**  
**18. Divisão, exílio e retorno.**

### BLOCO D — Profetas e esperança

**19. O que é profecia no próprio texto bíblico?**  
**20. Dia do Senhor, juízo e restauração.**  
**21. Servo, rei, sacerdote e Filho do Homem.**  
**22. Catálogo de profecias e relações messiânicas.**

O módulo atual de 357 relações será migrado para cá, mas cada entrada deverá receber classificação e contexto mais rigorosos.

### BLOCO E — Jesus

**23. Contexto narrativo dos Evangelhos.**  
**24. Nascimento e identidade.**  
**25. Reino de Deus.**  
**26. Sinais e obras.**  
**27. Ensinos e parábolas.**  
**28. Conflito, paixão e morte.**  
**29. Ressurreição.**  
**30. Ascensão e senhorio.**

### BLOCO F — Evangelho e comunidade

**31. Pecado, justificação, reconciliação e redenção.**  
**32. Fé, arrependimento e novo nascimento.**  
**33. Espírito Santo.**  
**34. Igreja e corpo de Cristo.**  
**35. Batismo e ceia conforme os textos que os tratam.**  
**36. Dons, serviço, liderança e disciplina.**  
**37. Ética, amor, justiça, dinheiro, sexualidade, família, trabalho e sofrimento.**

Temas controversos serão construídos por matriz de textos relevantes, sem iniciar pelo nome de uma posição denominacional.

### BLOCO G — Esperança e consumação

**38. Morte e ressurreição.**  
**39. Volta de Cristo.**  
**40. Juízo.**  
**41. Nova criação.**  
**42. Apocalipse em seu fluxo literário.**  
**43. Encerramento — Apocalipse 22:21.**

A numeração poderá aumentar à medida que módulos grandes forem subdivididos.

---

## 4. Sistema de evidências

Criar um registro estruturado para cada evidência externa:

```js
{
  id: "sennacherib-prism",
  type: "inscription",
  claim: "O prisma menciona Ezequias, rei de Judá, e tributo em 701 a.C.",
  biblical_refs: ["2Rs 18–19", "Is 36–37"],
  source_owner: "British Museum",
  source_url: "...",
  evidence_level: "direct-object-catalog",
  demonstrates: "...",
  does_not_demonstrate: "...",
  checked_at: "YYYY-MM-DD"
}
```

### Hierarquia preferida de fonte

1. imagem/digitalização do objeto ou manuscrito;
2. catálogo da instituição que conserva o objeto;
3. relatório/publicação arqueológica original;
4. edição crítica/base textual primária;
5. somente depois, material secundário para contexto — nunca como autoridade doutrinária.

Cada link deve receber data de última verificação em versões futuras.

---

## 5. Sistema de estudo bíblico

Estrutura proposta para dados de um estudo:

```js
{
  id: "fundamento-01",
  title: "O que pode ser testado empiricamente?",
  prerequisites: [],
  questions: [],
  passages: [],
  observations: [],
  internal_links: [],
  evidence: [],
  inferences: [],
  limits: [],
  conclusion: "",
  next: "fundamento-02"
}
```

### Regra para versículos

Fluxo de UI definitivo:

**TRADUÇÃO**  
→ seletor de versão  
→ **Ver texto original**  
→ seção original expandida  
→ botão **Estudar o original** no topo da seção  
→ painel lexical/morfológico/contextual

Nunca exigir que o estudante abra o original para compreender a tese principal.

### Traduções

- priorizar traduções cujo uso integral no site esteja juridicamente permitido;
- versões protegidas só entram com licença/API compatível;
- documentar versão, fonte e licença;
- manter seleção sincronizada entre passagens relacionadas quando isso melhorar comparação.

### Originais

- AT: hebraico/aramaico com corpus aberto e morfologia rastreável;
- NT: grego koiné com corpus aberto e morfologia rastreável;
- Strong pode ajudar navegação, mas não deve ser tratado como definição final do sentido;
- explicações lexicais devem ser subordinadas ao contexto sintático e literário.

---

## 6. UX / Design

### Identidade

Direção: **editorial contemporâneo + precisão tecnológica**.

Evitar:
- dashboard de aplicativo;
- cards excessivos;
- gradientes chamativos sem função;
- gamificação;
- aparência de blog religioso genérico;
- iconografia religiosa decorativa usada como substituto de conteúdo.

Usar:
- hierarquia tipográfica forte;
- espaços generosos;
- superfícies leves e sombras discretas;
- microinterações que indiquem relação e estado;
- animações curtas e funcionais;
- leitura excelente em telas estreitas;
- links e âncoras nativos da web;
- `prefers-reduced-motion`.

### Web primeiro

O projeto é um site. Portanto:
- cada estudo deve poder ter URL compartilhável;
- botão voltar deve respeitar histórico do navegador;
- conteúdo essencial não deve depender de gestos típicos de app;
- desktop, tablet e celular recebem layout responsivo, não telas de aplicativo adaptadas;
- PWA futura não altera a arquitetura editorial.

---

## 7. Estrutura técnica futura

A v0.1 continua deliberadamente simples: HTML/CSS/JS na raiz.

Quando o conteúdo crescer, migrar sem backend obrigatório para algo como:

```text
/index.html
/studies/*.json ou *.md
/data/scripture-*.json
/data/evidence.json
/js/*.js
/css/*.css
```

**Mas não fazer essa migração enquanto o upload móvel de ZIP na raiz for uma restrição operacional importante.** Para as versões iniciais, priorizar distribuição simples.

GitHub Pages continua como alvo principal.

---

## 8. Roadmap de implementação

### v0.1 — Fundação (esta entrega)
- manifesto;
- arquitetura visual do novo projeto;
- primeiro estudo empírico em versão inicial;
- trilha macro;
- fluxo tradução → original → estudo;
- módulo de profecias preservado;
- ZIP plano para upload móvel.

### v0.2 — Evidência textual
- expandir Fundamento 01;
- iniciar Fundamento 02 sobre manuscritos;
- criar componente padronizado de evidência;
- registrar data de verificação das fontes;
- criar sistema de notas de precisão/limite;
- melhorar deep links para capítulos e evidências.

### v0.3 — Motor de estudos
- transformar conteúdo em dados estruturados;
- navegação próxima/anterior entre estudos;
- progresso local opcional, sem conta;
- índice temático e busca global;
- glossário contextual de termos técnicos.

### v0.4 — Texto bíblico como infraestrutura
- leitor reutilizável em todos os estudos;
- referências cruzadas;
- seleção de tradução global;
- original lazy-load;
- análise termo a termo mais confiável;
- cache de corpus onde licenças permitirem.

### v0.5 — Profecias 2.0
- auditar as 357 relações;
- separar explicitamente: predição direta, citação explícita no NT, tipologia, alusão/eco, aplicação tradicional;
- contexto do AT antes do cumprimento;
- contexto do NT depois;
- reduzir dependência de listas tradicionais herdadas.

### v0.6–0.9 — Expansão da trilha
- preencher blocos A–D;
- testes editoriais e de coerência;
- auditoria de links/fontes;
- acessibilidade;
- performance móvel;
- PWA somente se não prejudicar a natureza de site.

### v1.0
Critério de “1.0” não é quantidade de páginas. É existir um **sistema editorial estável, auditável e reutilizável** no qual novos estudos possam ser acrescentados sem mudar as regras metodológicas.

---

## 9. Checklist para cada PR de conteúdo

- [ ] A pergunta do estudo está explícita.
- [ ] Todas as conclusões doutrinárias têm base bíblica exibida.
- [ ] O contexto imediato foi lido antes de usar versículo isolado.
- [ ] Relações AT/NT são classificadas corretamente.
- [ ] Nenhuma tradição, credo ou comentarista está sendo usado como autoridade da conclusão.
- [ ] Toda alegação material/histórica tem fonte rastreável.
- [ ] A fonte é o mais direta possível.
- [ ] “O que demonstra” está separado de “o que não demonstra”.
- [ ] Traduções e corpora têm licença/documentação.
- [ ] O estudo funciona no celular.
- [ ] Links e âncoras funcionam como web normal.
- [ ] Movimento respeita `prefers-reduced-motion`.
- [ ] Não existem erros JS no console.
- [ ] O próximo estudo depende apenas do que já foi construído.

---

## 10. Destino editorial

A trilha termina no encerramento do texto bíblico:

> Que a graça do Senhor Jesus seja com todos. Amém.

**Apocalipse 22:21**
