# PLANEJAMENTO — Scriptura v0.3

**Escopo desta versão:** corpus editorial executável com 1118 estudos unitários, arquitetura de UX, leitor bíblico interno, estudo do original, referências investigáveis e registro interno de fontes materiais/textuais. A opção editorial continua sendo **estudo guiado e estruturado**, não prosa ensaística inflada.


## 0. Estado da v0.3

A trilha deixou de ser apenas planejamento. Os **1118 estudos estão publicados como unidades estruturadas de investigação** em `estudos.js` e são renderizados pelo motor do `index.html`.

Cada unidade implementa o contrato editorial com: tema único, pergunta nuclear, referência ou objeto de análise, orientação, percurso de investigação, pontos de observação, síntese de controle, limites, relações internas, sequência e fontes externas quando aplicáveis. O progresso é local e cada estudo possui rota compartilhável `#estudo-NNN`.

A Bíblia funciona como infraestrutura interna do estudo. Uma referência abre o leitor contextual sem destruir o estado da página; a tradução vem primeiro, o original fica sob demanda e o estudo termo a termo só aparece a partir da seção original. Referências amplas oferecem navegação por livro/capítulo dentro do próprio site.

Para evidência externa, a v0.3 registra fichas de fontes custodiante/primárias e mostra internamente dado, escopo da evidência e limites antes do link oficial. A existência de um link nunca substitui o conteúdo investigável do painel.

**Definição de completo nesta fase:** nenhuma das 1118 entradas permanece como mero título ou placeholder. Completo não significa imutável: o corpus continua auditável e pode receber metadados mais precisos, novas fontes primárias, melhor glossário linguístico, fac-símiles legalmente incorporáveis e aprimoramentos de UX sem alterar o princípio metodológico.

## 1. Regras invioláveis

- **Um estudo = um tema nuclear.** Se o título puder ser naturalmente dividido em dois estudos, deve ser dividido.
- **Sola Scriptura para interpretação.** Fonte externa nunca encerra questão doutrinária.
- **Evidência direta para fatos externos.** Priorizar objeto, fac-símile, catálogo custodiante e publicação primária.
- **Referência é uma interação, não um hyperlink.** Primeiro abre investigação interna; o link oficial fica dentro do painel como auditoria.
- **UX é critério de aceite.** Conteúdo correto com fluxo ruim reprova a entrega.
- **Web first.** URL, hash, histórico, compartilhamento, acessibilidade, responsividade e SEO continuam nativos.
- **Sem prosa inflada.** Cada estudo deve avançar a investigação, não repetir manifesto ou introduções genéricas.
- **Conclusão proporcional.** Separar demonstrado, corroborado, plausível, incerto e não demonstrável.
- **Sem autoridade emprestada.** Credos, tradições, comentaristas e denominações podem ser objetos históricos, jamais fundamento hermenêutico.
- **Todo dado tem proveniência.** Corpus, tradução, imagem, objeto, transcrição e metadado precisam de origem/licença registradas.

## 2. Contrato de um estudo

Cada estudo é uma unidade navegável com URL própria e deve prever, na estrutura de dados:

```text
id · número · tema único · pergunta nuclear · pré-requisitos
texto-base · contexto imediato · contexto do livro
observações · relações internas · termos originais relevantes
evidências externas aplicáveis · inferências · limites
conclusão · questões em aberto · próximo estudo
```

O estudo não precisa exibir todas essas seções quando alguma não se aplica; o modelo existe para impedir saltos metodológicos.

## 3. Sistema interno de referências

### 3.1 Regra de interação
1. usuário ativa uma referência;
2. abre um painel contextual dentro do site;
3. o painel preserva o estudo e a posição de leitura;
4. o usuário investiga texto/objeto sem perder contexto;
5. fechar retorna exatamente ao ponto anterior;
6. “Abrir fonte oficial” é ação secundária, nunca a única forma de acesso.

### 3.2 Visualizadores previstos
- `BibleViewer`: tradução, versões, original, análise linguística, contexto, paralelos;
- `ManuscriptViewer`: fac-símile com zoom, transcrição alinhada, variantes, datação, custodiante;
- `InscriptionViewer`: imagem, recorte por linha, transliteração, tradução, aparato, proveniência;
- `ArtifactViewer`: fotos, medidas, material, datação, local de achado, local atual, cadeia de proveniência;
- `VariantViewer`: testemunhos lado a lado, diferença destacada, impacto de tradução;
- `TimelineViewer`: eventos e margens cronológicas;
- `MapViewer`: local bíblico, sítio arqueológico, rotas e camadas históricas;
- `CrossReferenceViewer`: textos lado a lado com correspondências realçadas;
- `SourceViewer`: instituição, item de acervo, licença, data de consulta, checksum/local mirror quando permitido.

### 3.3 Gate editorial de incorporação
Uma evidência essencial só entra em um estudo publicado quando o site consegue exibir internamente material suficiente para o leitor examiná-la: mídia licenciada/local, transcrição, metadados e contexto. Se isso não for legal ou tecnicamente possível, a evidência pode permanecer no backlog, mas não sustentar uma conclusão essencial.

## 4. UX como arquitetura

- **Camada 1 — Orientação:** onde estou, o que já sei, qual o próximo estudo.
- **Camada 2 — Leitura:** uma coluna principal, largura confortável, distração mínima.
- **Camada 3 — Investigação:** painéis contextuais sobre referências, sem navegação destrutiva.
- **Camada 4 — Comparação:** split view apenas quando comparar textos/objetos for a tarefa.
- **Camada 5 — Profundidade:** original, morfologia, variantes e metadados ficam sob demanda.
- **Mobile:** bottom sheet/overlay contextual com histórico próprio; nunca painel lateral espremido.
- **Desktop:** drawer ou split panel persistente, redimensionável quando útil.
- **Estado:** URL deve codificar estudo e referência aberta quando isso for compartilhável.
- **Busca:** busca global por tema, referência bíblica, pessoa, lugar, objeto, manuscrito e termo original.
- **Progressão:** marcar “não iniciado / em leitura / concluído” localmente, sem conta obrigatória.
- **Retomada:** salvar localmente último estudo e posição, sem sequestrar o botão voltar.
- **Acessibilidade:** teclado, foco, contraste, landmarks, labels, reduced motion, zoom de texto.
- **Performance:** shell rápido; dados pesados, fac-símiles e corpora carregados sob demanda.
- **Prazer:** microanimações funcionais, profundidade discreta, tipografia editorial, transições de contexto; nada ornamental que atrase leitura.

## 5. Trilha completa

**Total publicado nesta versão: 1118 estudos.** Blocos abaixo são apenas agrupadores de navegação; cada linha numerada é um estudo independente.

### Bloco A — Método de investigação

*Objetivo do bloco:* Definir como o projeto pergunta, observa, testa e limita conclusões.

- **001. O que é uma afirmação testável** — `1Ts 5:21`
- **002. O que é observação** — `At 17:11`
- **003. O que é inferência** — `Lc 10:26`
- **004. O que é conclusão** — `Jo 20:30-31`
- **005. O que é evidência direta** — `Jo 19:35`
- **006. O que é evidência indireta** — `Lc 1:1-4`
- **007. O que é testemunho** — `Dt 19:15`
- **008. O que é corroborar** — `2Co 13:1`
- **009. O que é contradição** — `Pv 18:17`
- **010. O que é ausência de evidência** — `Ec 3:11`
- **011. O que é proveniência de um objeto** — `Lc 1:1-4`
- **012. O que é datação** — `Lc 3:1-2`
- **013. O que é cadeia de custódia textual** — `Jr 36`
- **014. O que uma fonte primária pode demonstrar** — `Jo 19:35`
- **015. O que uma fonte primária não pode demonstrar** — `Jo 20:29`
- **016. Como registrar incerteza** — `1Co 13:9`
- **017. Como distinguir fato de interpretação** — `Ne 8:8`
- **018. Como comparar testemunhos independentes** — `Dt 19:15`
- **019. Como lidar com evidência conflitante** — `Pv 18:17`
- **020. Como revisar uma conclusão** — `At 18:24-26`

### Bloco B — Evidência material da Bíblia

*Objetivo do bloco:* Investigar objetos específicos e delimitar rigorosamente o que cada um sustenta.

- **021. Estela de Merneptá** — `Êx 1; Js 1`
- **022. Estela de Tel Dã** — `2Sm 7; 1Rs 12`
- **023. Estela de Mesa** — `2Rs 3`
- **024. Inscrição de Siloé** — `2Rs 20:20; 2Cr 32:30`
- **025. Túnel de Ezequias** — `2Rs 20:20`
- **026. Prisma de Senaqueribe** — `2Rs 18–19`
- **027. Relevos de Laquis** — `2Rs 18:13-17`
- **028. Crônica Babilônica da queda de Jerusalém** — `2Rs 24`
- **029. Tabletes de rações de Joaquim** — `2Rs 25:27-30`
- **030. Cilindro de Ciro** — `Ed 1`
- **031. Papiro de Elefantina** — `Ed 4–7`
- **032. Selos e bullae de Jerusalém** — `Jr 36`
- **033. Ketef Hinnom** — `Nm 6:24-26`
- **034. Grande Rolo de Isaías** — `Is`
- **035. Rolo de Habacuque** — `Hc`
- **036. Rolo do Templo** — `Êx–Dt`
- **037. Pedra de Pilatos** — `Mt 27`
- **038. Inscrição de Gálio** — `At 18:12-17`
- **039. Inscrição de Delfos** — `At 18:12-17`
- **040. Piscina de Betesda** — `Jo 5:2`
- **041. Piscina de Siloé** — `Jo 9:7`
- **042. Nazaret no registro arqueológico** — `Mt 2:23`
- **043. Cafarnaum no registro arqueológico** — `Mc 1:21`
- **044. Cesareia Marítima no registro arqueológico** — `At 10; 23–26`
- **045. Corinto no registro arqueológico** — `At 18`
- **046. Éfeso no registro arqueológico** — `At 19`
- **047. Areópago de Atenas** — `At 17:19`
- **048. Teatro de Éfeso** — `At 19:29`
- **049. Ossuário atribuído a Caifás** — `Mt 26:57`
- **050. Artefatos contestados como estudo de cautela** — `Pv 18:17`

### Bloco C — Transmissão do Antigo Testamento

*Objetivo do bloco:* Entender materialmente como o texto hebraico e aramaico chegou até nós.

- **051. O que é um manuscrito hebraico** — `Jr 36`
- **052. O que é um rolo** — `Jr 36:2`
- **053. O que é um códice**
- **054. O que são os Manuscritos do Mar Morto**
- **055. O que é 1QIsaᵃ** — `Is`
- **056. O que é o Texto Massorético**
- **057. O que é o Códice de Leningrado**
- **058. O que é o Códice de Aleppo**
- **059. O que é a Septuaginta como testemunho textual**
- **060. O que é o Pentateuco Samaritano**
- **061. O que é uma variante textual no AT**
- **062. O que é uma leitura consonantal**
- **063. O que são sinais massoréticos**
- **064. O que são notas massoréticas**
- **065. Como comparar dois testemunhos de Isaías** — `Is 53`
- **066. Como comparar dois testemunhos dos Salmos** — `Sl 22`
- **067. Como lacunas físicas afetam um manuscrito**
- **068. Como correções de escriba aparecem**
- **069. Como ortografia varia sem mudar o sentido**
- **070. Como uma variante pode afetar tradução**
- **071. Como uma variante pode não afetar tradução**
- **072. Como registrar variantes no site**
- **073. Como mostrar fac-símile e transcrição juntos**
- **074. Como separar texto preservado de reconstrução editorial**

### Bloco D — Transmissão do Novo Testamento

*Objetivo do bloco:* Entender os principais tipos de testemunhos gregos e sua comparação.

- **075. O que é um papiro do Novo Testamento**
- **076. O que é um uncial**
- **077. O que é um minúsculo**
- **078. O que é um lecionário**
- **079. Papiro P52** — `Jo 18`
- **080. Papiro P46** — `Rm–Hb`
- **081. Papiro P66** — `Jo`
- **082. Papiro P72** — `1Pe–Jd`
- **083. Papiro P75** — `Lc–Jo`
- **084. Codex Sinaiticus**
- **085. Codex Vaticanus**
- **086. Codex Alexandrinus**
- **087. Codex Bezae**
- **088. O que é uma variante textual no NT**
- **089. O que é transposição**
- **090. O que é omissão**
- **091. O que é adição**
- **092. O que é harmonização de copista**
- **093. O que é correção marginal**
- **094. Como comparar testemunhos de João 1** — `Jo 1`
- **095. Como comparar testemunhos de Marcos 16** — `Mc 16`
- **096. Como comparar testemunhos de João 7:53–8:11** — `Jo 7:53–8:11`
- **097. Como comparar testemunhos de 1 João 5:7-8** — `1Jo 5:7-8`
- **098. Como uma edição crítica registra variantes**
- **099. Como o site deve exibir incerteza textual**

### Bloco E — Tradução bíblica

*Objetivo do bloco:* Mostrar exatamente o que acontece quando o texto passa para outra língua.

- **100. O que é texto-fonte**
- **101. O que é língua-alvo**
- **102. O que é equivalência formal**
- **103. O que é equivalência funcional**
- **104. O que é tradução literal**
- **105. O que é tradução idiomática**
- **106. O que é ambiguidade lexical**
- **107. O que é ambiguidade sintática**
- **108. Como artigos gregos afetam tradução**
- **109. Como tempos verbais gregos afetam tradução**
- **110. Como aspectos verbais gregos afetam tradução**
- **111. Como estados construtos hebraicos afetam tradução**
- **112. Como paralelismo hebraico afeta tradução**
- **113. Como nomes divinos são traduzidos** — `Êx 3:14-15`
- **114. Como medidas antigas são traduzidas**
- **115. Como moedas antigas são traduzidas**
- **116. Como variantes entram em notas de tradução**
- **117. Como comparar versões sem escolher por preferência**
- **118. Como o seletor de versão deve funcionar**
- **119. Como documentar licença de cada tradução**

### Bloco F — A Escritura sobre a Escritura

*Objetivo do bloco:* Construir a doutrina do texto a partir de afirmações internas da própria Bíblia.

- **120. Inspiração da Escritura** — `2Tm 3:16`
- **121. Utilidade da Escritura** — `2Tm 3:16-17`
- **122. Suficiência para equipar** — `2Tm 3:17`
- **123. Palavra como verdade** — `Jo 17:17`
- **124. Palavra como luz** — `Sl 119:105`
- **125. Palavra como alimento** — `Dt 8:3; Mt 4:4`
- **126. Palavra como semente** — `Lc 8:11`
- **127. Palavra como espada** — `Hb 4:12`
- **128. Permanência da palavra** — `Is 40:8; 1Pe 1:25`
- **129. Não acrescentar à palavra** — `Dt 4:2`
- **130. Não retirar da palavra** — `Dt 4:2`
- **131. Examinar as Escrituras** — `At 17:11`
- **132. Ler publicamente a Escritura** — `1Tm 4:13`
- **133. Meditar na palavra** — `Sl 1`
- **134. Guardar a palavra** — `Sl 119:11`
- **135. Ensinar a palavra** — `Dt 6:6-7`
- **136. Obedecer à palavra** — `Tg 1:22`
- **137. Distorção da Escritura** — `2Pe 3:16`
- **138. Escritura interpretando Escritura** — `Lc 24:27`
- **139. Cumprimento das Escrituras** — `Lc 24:44`

### Bloco G — Cânon como objeto de investigação

*Objetivo do bloco:* Mapear o conjunto de livros sem transformar tradição posterior em autoridade doutrinária.

- **140. O que a Bíblia chama de Escrituras** — `2Tm 3:15`
- **141. A Lei como corpo textual** — `Js 1:8`
- **142. Os Profetas como corpo textual** — `Lc 24:27`
- **143. Os Salmos como corpo textual** — `Lc 24:44`
- **144. A tríade de Lucas 24:44** — `Lc 24:44`
- **145. Citações do AT por Jesus**
- **146. Citações do AT pelos apóstolos**
- **147. Fórmula “está escrito”**
- **148. Fórmula “a Escritura diz”**
- **149. Reconhecimento de cartas apostólicas** — `2Pe 3:15-16`
- **150. Leitura pública de cartas** — `Cl 4:16`
- **151. Circulação de cartas** — `Cl 4:16`
- **152. Apocalipse como profecia escrita** — `Ap 1:3`
- **153. Proibição final de acrescentar** — `Ap 22:18`
- **154. Proibição final de retirar** — `Ap 22:19`
- **155. Ordem dos livros como questão histórica**
- **156. Divisões judaicas do AT**
- **157. Divisões cristãs do AT**
- **158. Livros deuterocanônicos como questão de corpus**
- **159. Critérios do site para declarar escopo canônico**

### Bloco H — Leitura responsável

*Objetivo do bloco:* Ensinar ferramentas de leitura antes de conclusões doutrinárias.

- **160. Contexto do versículo**
- **161. Contexto do parágrafo**
- **162. Contexto da seção**
- **163. Contexto do livro**
- **164. Contexto canônico**
- **165. Quem fala no texto**
- **166. A quem o texto fala**
- **167. Quando o texto fala**
- **168. Onde o texto fala**
- **169. Por que o texto fala**
- **170. Narrativa**
- **171. Lei**
- **172. Poesia**
- **173. Sabedoria como princípio de leitura**
- **174. Profecia**
- **175. Evangelho**
- **176. Epístola**
- **177. Apocalíptica**
- **178. Metáfora**
- **179. Símile**
- **180. Hipérbole**
- **181. Ironia**
- **182. Paralelismo**
- **183. Quiasmo**
- **184. Citação explícita**
- **185. Alusão**
- **186. Eco textual**
- **187. Tipologia**
- **188. Promessa**
- **189. Cumprimento**
- **190. Lema**
- **191. Forma flexionada**
- **192. Campo semântico**
- **193. Sintaxe**
- **194. Morfologia**
- **195. Falácia da raiz**
- **196. Falácia do Strong**
- **197. Anacronismo semântico**
- **198. Descrição versus prescrição**
- **199. Silêncio do texto**

### Bloco I — Criação

*Objetivo do bloco:* Investigar cada afirmação fundamental de Gênesis 1–2 separadamente.

- **200. Deus como Criador** — `Gn 1:1`
- **201. Criação dos céus** — `Gn 1:1`
- **202. Criação da terra** — `Gn 1:1`
- **203. Luz** — `Gn 1:3-5`
- **204. Firmamento** — `Gn 1:6-8`
- **205. Terra seca** — `Gn 1:9-10`
- **206. Vegetação** — `Gn 1:11-13`
- **207. Luminares** — `Gn 1:14-19`
- **208. Animais aquáticos** — `Gn 1:20-23`
- **209. Animais terrestres** — `Gn 1:24-25`
- **210. Humanidade** — `Gn 1:26-27`
- **211. Imagem de Deus** — `Gn 1:26-27`
- **212. Domínio humano** — `Gn 1:28`
- **213. Alimento original** — `Gn 1:29-30`
- **214. Bondade da criação** — `Gn 1:31`
- **215. Sétimo dia** — `Gn 2:1-3`
- **216. Pó da terra** — `Gn 2:7`
- **217. Fôlego de vida** — `Gn 2:7`
- **218. Jardim do Éden** — `Gn 2:8`
- **219. Árvore da vida no Éden** — `Gn 2:9`
- **220. Árvore do conhecimento** — `Gn 2:9`
- **221. Mandato do jardim** — `Gn 2:15`
- **222. Proibição do fruto** — `Gn 2:16-17`
- **223. Formação da mulher** — `Gn 2:21-22`
- **224. Uma só carne** — `Gn 2:24`
- **225. Nudez sem vergonha** — `Gn 2:25`

### Bloco J — Queda e primeiros juízos

*Objetivo do bloco:* Acompanhar cada elemento da ruptura de Gênesis 3–11.

- **226. A serpente** — `Gn 3:1`
- **227. A tentação** — `Gn 3:1-5`
- **228. O primeiro pecado humano** — `Gn 3:6`
- **229. Vergonha** — `Gn 3:7`
- **230. Esconder-se de Deus** — `Gn 3:8`
- **231. Interrogatório divino** — `Gn 3:9-13`
- **232. Juízo da serpente** — `Gn 3:14`
- **233. Inimizade das sementes** — `Gn 3:15`
- **234. Dor da mulher** — `Gn 3:16`
- **235. Dominação no relacionamento** — `Gn 3:16`
- **236. Maldição do solo** — `Gn 3:17`
- **237. Trabalho penoso** — `Gn 3:17-19`
- **238. Morte** — `Gn 3:19`
- **239. Vestes de pele** — `Gn 3:21`
- **240. Expulsão do Éden** — `Gn 3:22-24`
- **241. Caim** — `Gn 4`
- **242. Abel** — `Gn 4`
- **243. Oferta rejeitada de Caim** — `Gn 4:5`
- **244. Sangue de Abel** — `Gn 4:10`
- **245. Marca de Caim** — `Gn 4:15`
- **246. Violência de Lameque** — `Gn 4:23-24`
- **247. Genealogia de Adão** — `Gn 5`
- **248. Corrupção antes do dilúvio** — `Gn 6:5`
- **249. Noé encontrou graça** — `Gn 6:8`
- **250. Dilúvio** — `Gn 6–8`
- **251. Arca** — `Gn 6–8`
- **252. Aliança com Noé** — `Gn 9`
- **253. Sinal do arco** — `Gn 9:12-17`
- **254. Valor do sangue humano** — `Gn 9:5-6`
- **255. Nações de Gênesis 10** — `Gn 10`
- **256. Babel** — `Gn 11:1-9`
- **257. Confusão das línguas** — `Gn 11:7-9`

### Bloco K — Abraão

*Objetivo do bloco:* Seguir separadamente as promessas e respostas na narrativa de Abraão.

- **258. Chamado de Abrão** — `Gn 12:1`
- **259. Terra prometida a Abrão** — `Gn 12:1`
- **260. Grande nação prometida** — `Gn 12:2`
- **261. Grande nome prometido** — `Gn 12:2`
- **262. Bênção às famílias da terra** — `Gn 12:3`
- **263. Altares de Abrão** — `Gn 12`
- **264. Abrão no Egito** — `Gn 12:10-20`
- **265. Separação de Ló** — `Gn 13`
- **266. Promessa da descendência numerosa** — `Gn 13:16`
- **267. Melquisedeque** — `Gn 14:18-20`
- **268. Dízimo de Abrão** — `Gn 14:20`
- **269. Fé creditada como justiça** — `Gn 15:6`
- **270. Aliança de Gênesis 15** — `Gn 15`
- **271. Hagar** — `Gn 16`
- **272. Ismael** — `Gn 16–17`
- **273. Mudança do nome Abraão** — `Gn 17:5`
- **274. Circuncisão** — `Gn 17:10-14`
- **275. Promessa de Isaque** — `Gn 17:19`
- **276. Intercessão por Sodoma** — `Gn 18`
- **277. Juízo de Sodoma** — `Gn 19`
- **278. Nascimento de Isaque** — `Gn 21`
- **279. Expulsão de Hagar** — `Gn 21`
- **280. Sacrifício de Isaque** — `Gn 22`
- **281. O Senhor proverá** — `Gn 22:14`
- **282. Juramento após Moriá** — `Gn 22:16-18`
- **283. Sepultura de Sara** — `Gn 23`

### Bloco L — Isaque, Jacó e José

*Objetivo do bloco:* Completar os fundamentos patriarcais sem condensar personagens distintos.

- **284. Isaque como filho da promessa** — `Gn 21`
- **285. Rebeca** — `Gn 24`
- **286. Esaú** — `Gn 25`
- **287. Jacó** — `Gn 25`
- **288. Primogenitura** — `Gn 25:29-34`
- **289. Bênção de Isaque** — `Gn 27`
- **290. Escada de Betel** — `Gn 28`
- **291. Promessa a Jacó** — `Gn 28:13-15`
- **292. Lia** — `Gn 29`
- **293. Raquel** — `Gn 29`
- **294. Doze filhos de Jacó** — `Gn 29–30`
- **295. Luta de Jacó** — `Gn 32`
- **296. Nome Israel** — `Gn 32:28`
- **297. Reconciliação com Esaú** — `Gn 33`
- **298. José vendido** — `Gn 37`
- **299. José no Egito** — `Gn 39`
- **300. José e os sonhos** — `Gn 40–41`
- **301. José como governador** — `Gn 41`
- **302. Fome** — `Gn 41–47`
- **303. Reconciliação de José** — `Gn 45`
- **304. Providência em Gênesis 50:20** — `Gn 50:20`
- **305. Bênção de Judá** — `Gn 49:8-12`
- **306. Cetro de Judá** — `Gn 49:10`
- **307. Morte de José** — `Gn 50`

### Bloco M — Êxodo

*Objetivo do bloco:* Investigar a libertação do Egito em unidades conceituais independentes.

- **308. Escravidão no Egito** — `Êx 1`
- **309. Nascimento de Moisés** — `Êx 2`
- **310. Sarça ardente** — `Êx 3`
- **311. Nome YHWH** — `Êx 3:14-15`
- **312. Chamado de Moisés** — `Êx 3–4`
- **313. Faraó endurecido** — `Êx 4–14`
- **314. Sinais diante de Faraó** — `Êx 7`
- **315. Águas em sangue** — `Êx 7`
- **316. Rãs** — `Êx 8`
- **317. Piolhos** — `Êx 8`
- **318. Moscas** — `Êx 8`
- **319. Peste nos animais** — `Êx 9`
- **320. Úlceras** — `Êx 9`
- **321. Granizo** — `Êx 9`
- **322. Gafanhotos** — `Êx 10`
- **323. Trevas** — `Êx 10`
- **324. Morte dos primogênitos** — `Êx 11–12`
- **325. Páscoa** — `Êx 12`
- **326. Cordeiro pascal** — `Êx 12`
- **327. Sangue nos umbrais** — `Êx 12:7`
- **328. Pães sem fermento** — `Êx 12`
- **329. Consagração dos primogênitos** — `Êx 13`
- **330. Coluna de nuvem** — `Êx 13`
- **331. Coluna de fogo** — `Êx 13`
- **332. Travessia do mar** — `Êx 14`
- **333. Cântico de Moisés** — `Êx 15`
- **334. Maná** — `Êx 16`
- **335. Água da rocha** — `Êx 17`
- **336. Batalha com Amaleque** — `Êx 17`
- **337. Conselho de Jetro** — `Êx 18`

### Bloco N — Sinai e mandamentos

*Objetivo do bloco:* Separar aliança, mediação e cada mandamento fundamental.

- **338. Chegada ao Sinai** — `Êx 19`
- **339. Reino de sacerdotes** — `Êx 19:6`
- **340. Santidade da assembleia** — `Êx 19`
- **341. Mediação de Moisés** — `Êx 19–20`
- **342. Não ter outros deuses** — `Êx 20:3`
- **343. Não fazer ídolos** — `Êx 20:4-6`
- **344. Não tomar o nome em vão** — `Êx 20:7`
- **345. Guardar o sábado** — `Êx 20:8-11`
- **346. Honrar pai e mãe** — `Êx 20:12`
- **347. Não matar** — `Êx 20:13`
- **348. Não adulterar** — `Êx 20:14`
- **349. Não furtar** — `Êx 20:15`
- **350. Não dar falso testemunho** — `Êx 20:16`
- **351. Não cobiçar** — `Êx 20:17`
- **352. Livro da Aliança** — `Êx 21–23`
- **353. Ratificação da aliança** — `Êx 24`
- **354. Sangue da aliança** — `Êx 24:8`
- **355. Tábuas de pedra** — `Êx 24:12`
- **356. Bezerro de ouro** — `Êx 32`
- **357. Intercessão de Moisés** — `Êx 32`
- **358. Presença de Deus** — `Êx 33`
- **359. Glória de Deus** — `Êx 33–34`
- **360. Renovação da aliança** — `Êx 34`
- **361. Rosto resplandecente de Moisés** — `Êx 34:29-35`

### Bloco O — Tabernáculo

*Objetivo do bloco:* Estudar cada componente do santuário como tema próprio antes de qualquer leitura tipológica.

- **362. Propósito do tabernáculo** — `Êx 25:8`
- **363. Arca da aliança** — `Êx 25:10-22`
- **364. Propiciatório** — `Êx 25:17-22`
- **365. Querubins** — `Êx 25:18-22`
- **366. Mesa dos pães** — `Êx 25:23-30`
- **367. Pães da presença** — `Lv 24:5-9`
- **368. Candelabro** — `Êx 25:31-40`
- **369. Cortinas do tabernáculo** — `Êx 26`
- **370. Véu** — `Êx 26:31-33`
- **371. Altar de bronze** — `Êx 27:1-8`
- **372. Átrio** — `Êx 27:9-19`
- **373. Óleo da lâmpada** — `Êx 27:20-21`
- **374. Altar do incenso** — `Êx 30:1-10`
- **375. Incenso** — `Êx 30:34-38`
- **376. Bacia de bronze** — `Êx 30:17-21`
- **377. Óleo da unção** — `Êx 30:22-33`
- **378. Sábado na construção** — `Êx 31:12-17`
- **379. Bezalel** — `Êx 31:1-5`
- **380. Ooliabe** — `Êx 31:6`
- **381. Glória enchendo o tabernáculo** — `Êx 40:34-38`

### Bloco P — Sacerdócio e sacrifícios

*Objetivo do bloco:* Tratar cada função e oferta sem fundi-las.

- **382. Arão como sumo sacerdote** — `Êx 28`
- **383. Vestes sacerdotais** — `Êx 28`
- **384. Peitoral** — `Êx 28:15-30`
- **385. Urim e Tumim** — `Êx 28:30`
- **386. Consagração sacerdotal** — `Êx 29`
- **387. Sacerdócio levítico** — `Nm 18`
- **388. Holocausto** — `Lv 1`
- **389. Oferta de cereal** — `Lv 2`
- **390. Oferta pacífica** — `Lv 3`
- **391. Oferta pelo pecado** — `Lv 4`
- **392. Oferta pela culpa** — `Lv 5`
- **393. Sangue no sistema sacrificial** — `Lv 17:11`
- **394. Imposição de mãos** — `Lv 1:4`
- **395. Fogo contínuo do altar** — `Lv 6:12-13`
- **396. Animais limpos** — `Lv 11`
- **397. Animais impuros** — `Lv 11`
- **398. Pureza ritual** — `Lv 11–15`
- **399. Santidade** — `Lv 19:2`
- **400. Dia da Expiação** — `Lv 16`
- **401. Bode para o Senhor** — `Lv 16`
- **402. Bode emissário** — `Lv 16`
- **403. Entrada no Santo dos Santos** — `Lv 16`
- **404. Expiação anual** — `Lv 16:34`
- **405. Páscoa em Levítico** — `Lv 23:4-5`
- **406. Pães Asmos** — `Lv 23:6-8`
- **407. Primícias** — `Lv 23:9-14`
- **408. Semanas** — `Lv 23:15-22`
- **409. Trombetas** — `Lv 23:23-25`
- **410. Dia da Expiação no calendário** — `Lv 23:26-32`
- **411. Tabernáculos** — `Lv 23:33-43`
- **412. Ano sabático** — `Lv 25:1-7`
- **413. Jubileu** — `Lv 25:8-55`
- **414. Resgatador** — `Lv 25:25`
- **415. Amar o próximo** — `Lv 19:18`

### Bloco Q — Deserto e Deuteronômio

*Objetivo do bloco:* Mapear testes, rebeliões e renovação da aliança.

- **416. Censo de Israel** — `Nm 1`
- **417. Acampamento de Israel** — `Nm 2`
- **418. Nazireado** — `Nm 6`
- **419. Bênção sacerdotal** — `Nm 6:24-26`
- **420. Nuvem sobre o tabernáculo** — `Nm 9`
- **421. Trombetas de prata** — `Nm 10`
- **422. Murmuração** — `Nm 11`
- **423. Setenta anciãos** — `Nm 11`
- **424. Espírito sobre os anciãos** — `Nm 11:25`
- **425. Espias da terra** — `Nm 13`
- **426. Incredulidade em Cades** — `Nm 14`
- **427. Quarenta anos no deserto** — `Nm 14`
- **428. Rebelião de Corá** — `Nm 16`
- **429. Vara de Arão** — `Nm 17`
- **430. Águas de Meribá** — `Nm 20`
- **431. Serpentes ardentes** — `Nm 21`
- **432. Serpente de bronze** — `Nm 21:8-9`
- **433. Balaão** — `Nm 22–24`
- **434. Estrela de Jacó** — `Nm 24:17`
- **435. Segunda geração** — `Nm 26`
- **436. Shema** — `Dt 6:4-5`
- **437. Ensino aos filhos** — `Dt 6:6-9`
- **438. Profeta semelhante a Moisés** — `Dt 18:15-19`
- **439. Teste do profeta** — `Dt 13`
- **440. Cidades de refúgio** — `Dt 19`
- **441. Bênçãos da aliança** — `Dt 28`
- **442. Maldições da aliança** — `Dt 28`
- **443. Circuncisão do coração** — `Dt 30:6`
- **444. Escolher a vida** — `Dt 30:19`
- **445. Morte de Moisés** — `Dt 34`

### Bloco R — Terra, juízes e Rute

*Objetivo do bloco:* Acompanhar a entrada na terra e a crise pré-monárquica.

- **446. Josué como sucessor** — `Js 1`
- **447. Travessia do Jordão** — `Js 3`
- **448. Pedras memoriais** — `Js 4`
- **449. Jericó** — `Js 6`
- **450. Raabe** — `Js 2; 6`
- **451. Pecado de Acã** — `Js 7`
- **452. Aliança em Siquém** — `Js 24`
- **453. Distribuição da terra** — `Js 13–21`
- **454. Descanso na terra** — `Js 21:44`
- **455. Ciclo dos juízes** — `Jz 2`
- **456. Débora** — `Jz 4–5`
- **457. Gideão** — `Jz 6–8`
- **458. Jefté** — `Jz 11`
- **459. Sansão** — `Jz 13–16`
- **460. Ausência de rei** — `Jz 21:25`
- **461. Rute** — `Rt`
- **462. Noemi** — `Rt`
- **463. Boaz** — `Rt`
- **464. Resgatador em Rute** — `Rt 4`
- **465. Linhagem de Davi em Rute** — `Rt 4:17-22`

### Bloco S — Reino

*Objetivo do bloco:* Investigar a monarquia e a promessa davídica passo a passo.

- **466. Samuel** — `1Sm 1–3`
- **467. Pedido por um rei** — `1Sm 8`
- **468. Saul** — `1Sm 9–31`
- **469. Obediência acima do sacrifício** — `1Sm 15:22`
- **470. Davi ungido** — `1Sm 16`
- **471. Davi e Golias** — `1Sm 17`
- **472. Aliança de Jônatas** — `1Sm 18–20`
- **473. Davi poupando Saul** — `1Sm 24`
- **474. Davi rei** — `2Sm 5`
- **475. Jerusalém como capital** — `2Sm 5:6-10`
- **476. Arca em Jerusalém** — `2Sm 6`
- **477. Promessa de 2 Samuel 7** — `2Sm 7`
- **478. Casa prometida a Davi** — `2Sm 7:11`
- **479. Descendente prometido a Davi** — `2Sm 7:12`
- **480. Trono eterno prometido** — `2Sm 7:13,16`
- **481. Pecado de Davi** — `2Sm 11`
- **482. Confronto de Natã** — `2Sm 12`
- **483. Absalão** — `2Sm 15–18`
- **484. Salomão** — `1Rs 1–11`
- **485. Pedido de sabedoria** — `1Rs 3`
- **486. Construção do templo** — `1Rs 5–6`
- **487. Dedicação do templo** — `1Rs 8`
- **488. Glória no templo** — `1Rs 8:10-11`
- **489. Rainha de Sabá** — `1Rs 10`
- **490. Apostasia de Salomão** — `1Rs 11`
- **491. Divisão do reino** — `1Rs 12`
- **492. Jeroboão** — `1Rs 12`
- **493. Bezerros de Betel e Dã** — `1Rs 12:28-33`
- **494. Elias** — `1Rs 17–19`
- **495. Monte Carmelo** — `1Rs 18`
- **496. Eliseu** — `2Rs 2–13`
- **497. Queda de Samaria** — `2Rs 17`
- **498. Ezequias** — `2Rs 18–20`
- **499. Josias** — `2Rs 22–23`
- **500. Livro encontrado no templo** — `2Rs 22`
- **501. Queda de Jerusalém** — `2Rs 25`
- **502. Exílio babilônico** — `2Rs 25`
- **503. Libertação de Joaquim** — `2Rs 25:27-30`

### Bloco T — Sabedoria e poesia

*Objetivo do bloco:* Estudar categorias sapienciais e poéticas sem confundi-las com promessas proféticas.

- **504. Temor do Senhor** — `Pv 1:7`
- **505. Sabedoria personificada em Provérbios 8** — `Pv 8`
- **506. Insensatez** — `Pv`
- **507. Justiça em Provérbios** — `Pv`
- **508. Preguiça** — `Pv 6:6-11`
- **509. Palavras** — `Pv 18:21`
- **510. Dinheiro em Provérbios** — `Pv 11`
- **511. Pobre em Provérbios** — `Pv 14:31`
- **512. Disciplina em Provérbios** — `Pv 3:11-12`
- **513. Amizade em Provérbios** — `Pv 17:17`
- **514. Casamento em Provérbios** — `Pv 5`
- **515. Mulher virtuosa** — `Pv 31`
- **516. Sofrimento de Jó** — `Jó`
- **517. Acusador em Jó** — `Jó 1–2`
- **518. Integridade de Jó** — `Jó 1:1`
- **519. Limites humanos em Jó** — `Jó 38–42`
- **520. Vaidade em Eclesiastes** — `Ec 1`
- **521. Tempo em Eclesiastes** — `Ec 3`
- **522. Temor de Deus em Eclesiastes** — `Ec 12:13`
- **523. Amor no Cântico** — `Ct`
- **524. Bem-aventurado do Salmo 1** — `Sl 1`
- **525. Rei ungido do Salmo 2** — `Sl 2`
- **526. Pastor do Salmo 23** — `Sl 23`
- **527. Sofrimento do Salmo 22** — `Sl 22`
- **528. Perdão no Salmo 32** — `Sl 32`
- **529. Arrependimento no Salmo 51** — `Sl 51`
- **530. Reinado do Senhor nos Salmos** — `Sl 93–99`
- **531. Sacerdote do Salmo 110** — `Sl 110`
- **532. Palavra no Salmo 119** — `Sl 119`
- **533. Aleluia nos Salmos finais** — `Sl 146–150`

### Bloco U — Profetas

*Objetivo do bloco:* Construir a esperança profética a partir de temas isolados.

- **534. Chamado de Isaías** — `Is 6`
- **535. Santo de Israel** — `Is`
- **536. Sinal de Emanuel** — `Is 7:14`
- **537. Filho de Isaías 9** — `Is 9:6-7`
- **538. Renovo de Jessé em Isaías 11** — `Is 11`
- **539. Remanescente** — `Is 10–11`
- **540. Servo de Isaías 42** — `Is 42`
- **541. Servo de Isaías 49** — `Is 49`
- **542. Servo de Isaías 50** — `Is 50`
- **543. Servo de Isaías 52–53** — `Is 52:13–53:12`
- **544. Boas-novas de Isaías 61** — `Is 61`
- **545. Novo êxodo em Isaías** — `Is 40–55`
- **546. Novos céus em Isaías** — `Is 65:17`
- **547. Nova terra em Isaías** — `Is 65:17`
- **548. Chamado de Jeremias** — `Jr 1`
- **549. Templo em Jeremias 7** — `Jr 7`
- **550. Renovo justo de Jeremias** — `Jr 23:5-6`
- **551. Nova aliança** — `Jr 31:31-34`
- **552. Lei no coração** — `Jr 31:33`
- **553. Perdão na nova aliança** — `Jr 31:34`
- **554. Novo coração em Ezequiel** — `Ez 36:26`
- **555. Novo espírito em Ezequiel** — `Ez 36:26`
- **556. Espírito de Deus em Ezequiel 36** — `Ez 36:27`
- **557. Vale de ossos secos** — `Ez 37`
- **558. Um só pastor em Ezequiel 34** — `Ez 34:23`
- **559. Templo de Ezequiel** — `Ez 40–48`
- **560. Filho do Homem em Daniel 7** — `Dn 7:13-14`
- **561. Quatro reinos em Daniel 7** — `Dn 7`
- **562. Setenta semanas** — `Dn 9:24-27`
- **563. Ressurreição em Daniel 12** — `Dn 12:2`
- **564. Amor pactual em Oseias** — `Os`
- **565. Chamado do Egito em Oseias** — `Os 11:1`
- **566. Derramamento do Espírito em Joel** — `Jl 2:28-32`
- **567. Dia do Senhor em Joel** — `Jl 2`
- **568. Justiça em Amós** — `Am 5:24`
- **569. Belém em Miqueias** — `Mq 5:2`
- **570. Justiça em Miqueias** — `Mq 6:8`
- **571. Justo pela fé em Habacuque** — `Hc 2:4`
- **572. Restauração em Sofonias** — `Sf 3`
- **573. Glória do segundo templo em Ageu** — `Ag 2`
- **574. Renovo em Zacarias 3** — `Zc 3:8`
- **575. Rei humilde em Zacarias 9** — `Zc 9:9`
- **576. Trinta moedas em Zacarias 11** — `Zc 11:12-13`
- **577. Traspassado em Zacarias 12** — `Zc 12:10`
- **578. Pastor ferido em Zacarias 13** — `Zc 13:7`
- **579. Mensageiro em Malaquias 3** — `Ml 3:1`
- **580. Elias em Malaquias 4** — `Ml 4:5-6`

### Bloco V — Messias nas Escrituras

*Objetivo do bloco:* Reunir linhas messiânicas como estudos independentes antes do catálogo de correspondências.

- **581. Descendente da mulher** — `Gn 3:15`
- **582. Descendente de Abraão** — `Gn 22:18`
- **583. Descendente de Isaque** — `Gn 21:12`
- **584. Descendente de Jacó** — `Nm 24:17`
- **585. Descendente de Judá** — `Gn 49:10`
- **586. Descendente de Davi** — `2Sm 7:12-16`
- **587. Rei ungido** — `Sl 2`
- **588. Filho no Salmo 2** — `Sl 2:7`
- **589. Herdeiro das nações** — `Sl 2:8`
- **590. Homem ideal do Salmo 8** — `Sl 8`
- **591. Sofredor do Salmo 22** — `Sl 22`
- **592. Santo que não vê corrupção** — `Sl 16:10`
- **593. Rei justo do Salmo 45** — `Sl 45`
- **594. Rei universal do Salmo 72** — `Sl 72`
- **595. Pedra rejeitada** — `Sl 118:22`
- **596. Sacerdote segundo Melquisedeque** — `Sl 110:4`
- **597. Senhor à direita de Deus** — `Sl 110:1`
- **598. Emanuel** — `Is 7:14`
- **599. Filho governante** — `Is 9:6-7`
- **600. Renovo de Jessé na leitura messiânica** — `Is 11:1`
- **601. Servo escolhido** — `Is 42:1`
- **602. Luz das nações** — `Is 49:6`
- **603. Servo obediente** — `Is 50:5-6`
- **604. Servo exaltado** — `Is 52:13`
- **605. Servo desprezado** — `Is 53:3`
- **606. Servo traspassado** — `Is 53:5`
- **607. Servo substitutivo** — `Is 53:5-6`
- **608. Servo silencioso** — `Is 53:7`
- **609. Servo sepultado com rico** — `Is 53:9`
- **610. Servo justificador** — `Is 53:11`
- **611. Servo intercessor** — `Is 53:12`
- **612. Renovo justo** — `Jr 23:5`
- **613. Senhor Justiça Nossa** — `Jr 23:6`
- **614. Pastor davídico** — `Ez 34:23`
- **615. Filho do Homem entronizado** — `Dn 7:13-14`
- **616. Ungido de Daniel 9** — `Dn 9:25-26`
- **617. Governante de Belém** — `Mq 5:2`
- **618. Rei humilde** — `Zc 9:9`
- **619. Rei montado em jumento** — `Zc 9:9`
- **620. Traspassado** — `Zc 12:10`
- **621. Pastor ferido** — `Zc 13:7`
- **622. Mensageiro da aliança** — `Ml 3:1`
- **623. Precursor** — `Ml 3:1; 4:5`
- **624. Catálogo AT → NT como ferramenta** — `Lc 24:27,44`

### Bloco W — Nascimento e identidade de Jesus

*Objetivo do bloco:* Entrar nos Evangelhos por afirmações de identidade, uma por vez.

- **625. Genealogia de Mateus** — `Mt 1:1-17`
- **626. Genealogia de Lucas** — `Lc 3:23-38`
- **627. Concepção de Jesus** — `Mt 1:18-25`
- **628. Nascimento virginal** — `Mt 1:18-25; Lc 1:26-35`
- **629. Nome Jesus** — `Mt 1:21`
- **630. Emanuel em Mateus** — `Mt 1:23`
- **631. Nascimento em Belém** — `Mt 2:1`
- **632. Magos** — `Mt 2`
- **633. Fuga para o Egito** — `Mt 2:13-15`
- **634. Matança dos meninos** — `Mt 2:16-18`
- **635. Retorno a Nazaré** — `Mt 2:19-23`
- **636. Anúncio a Zacarias** — `Lc 1`
- **637. Nascimento de João Batista** — `Lc 1`
- **638. Anunciação a Maria** — `Lc 1:26-38`
- **639. Magnificat** — `Lc 1:46-55`
- **640. Nascimento de Jesus em Lucas** — `Lc 2`
- **641. Pastores em Belém** — `Lc 2:8-20`
- **642. Simeão** — `Lc 2:25-35`
- **643. Ana** — `Lc 2:36-38`
- **644. Jesus no templo aos doze anos** — `Lc 2:41-52`
- **645. Prólogo de João** — `Jo 1:1-18`
- **646. O Verbo** — `Jo 1:1`
- **647. O Verbo com Deus** — `Jo 1:1`
- **648. O Verbo era Deus** — `Jo 1:1`
- **649. O Verbo se fez carne** — `Jo 1:14`
- **650. Unigênito** — `Jo 1:14,18`
- **651. Cordeiro de Deus** — `Jo 1:29`
- **652. Filho de Deus** — `Jo 1:34`
- **653. Filho do Homem** — `Jo 1:51`
- **654. Messias** — `Jo 1:41`

### Bloco X — Preparação e início do ministério

*Objetivo do bloco:* Estudar os eventos inaugurais do ministério de Jesus.

- **655. João Batista no deserto** — `Mt 3`
- **656. Batismo de arrependimento** — `Mc 1:4`
- **657. Batismo de Jesus** — `Mt 3:13-17`
- **658. Voz do céu no batismo** — `Mt 3:17`
- **659. Espírito no batismo** — `Mt 3:16`
- **660. Tentação no deserto** — `Mt 4:1-11`
- **661. Primeira tentação** — `Mt 4:3-4`
- **662. Segunda tentação** — `Mt 4:5-7`
- **663. Terceira tentação** — `Mt 4:8-10`
- **664. Retorno à Galileia** — `Mt 4:12`
- **665. Chamado de Pedro** — `Mt 4:18-20`
- **666. Chamado de André** — `Mt 4:18-20`
- **667. Chamado de Tiago** — `Mt 4:21-22`
- **668. Chamado de João** — `Mt 4:21-22`
- **669. Chamado de Mateus** — `Mt 9:9`
- **670. Chamado de Filipe** — `Jo 1:43`
- **671. Natanael** — `Jo 1:45-51`
- **672. Bodas de Caná** — `Jo 2:1-11`
- **673. Primeira purificação do templo em João** — `Jo 2:13-22`
- **674. Nicodemos** — `Jo 3`
- **675. Mulher samaritana** — `Jo 4`
- **676. Testemunho em Samaria** — `Jo 4:39-42`

### Bloco Y — Ensino de Jesus

*Objetivo do bloco:* Separar conceitos centrais do ensino de Jesus.

- **677. Reino dos céus** — `Mt`
- **678. Reino de Deus** — `Mc; Lc`
- **679. Arrependimento no ensino de Jesus** — `Mt 4:17`
- **680. Fé no ensino de Jesus** — `Mc 1:15`
- **681. Novo nascimento no ensino de Jesus** — `Jo 3:3-8`
- **682. Água viva** — `Jo 4:10-14`
- **683. Pão da vida** — `Jo 6:35`
- **684. Luz do mundo** — `Jo 8:12`
- **685. Porta das ovelhas** — `Jo 10:7`
- **686. Bom Pastor** — `Jo 10:11`
- **687. Ressurreição e vida** — `Jo 11:25`
- **688. Caminho** — `Jo 14:6`
- **689. Verdade** — `Jo 14:6`
- **690. Vida** — `Jo 14:6`
- **691. Videira verdadeira** — `Jo 15:1`
- **692. Bem-aventurados os pobres em espírito** — `Mt 5:3`
- **693. Bem-aventurados os que choram** — `Mt 5:4`
- **694. Bem-aventurados os mansos** — `Mt 5:5`
- **695. Bem-aventurados os famintos de justiça** — `Mt 5:6`
- **696. Bem-aventurados os misericordiosos** — `Mt 5:7`
- **697. Bem-aventurados os limpos de coração** — `Mt 5:8`
- **698. Bem-aventurados os pacificadores** — `Mt 5:9`
- **699. Bem-aventurados os perseguidos** — `Mt 5:10`
- **700. Sal da terra** — `Mt 5:13`
- **701. Luz do mundo nos discípulos** — `Mt 5:14-16`
- **702. Jesus e a Lei** — `Mt 5:17-20`
- **703. Ira no Sermão do Monte** — `Mt 5:21-26`
- **704. Adultério do coração** — `Mt 5:27-30`
- **705. Divórcio no Sermão do Monte** — `Mt 5:31-32`
- **706. Juramentos** — `Mt 5:33-37`
- **707. Não resistir ao perverso** — `Mt 5:38-42`
- **708. Amar inimigos** — `Mt 5:43-48`
- **709. Esmolas em secreto** — `Mt 6:1-4`
- **710. Oração em secreto** — `Mt 6:5-8`
- **711. Pai nosso** — `Mt 6:9-13`
- **712. Jejum em secreto** — `Mt 6:16-18`
- **713. Tesouros no céu** — `Mt 6:19-21`
- **714. Olho como lâmpada** — `Mt 6:22-23`
- **715. Dois senhores** — `Mt 6:24`
- **716. Ansiedade no ensino de Jesus** — `Mt 6:25-34`
- **717. Julgar** — `Mt 7:1-5`
- **718. Pérolas aos porcos** — `Mt 7:6`
- **719. Pedir buscar bater** — `Mt 7:7-11`
- **720. Regra de ouro** — `Mt 7:12`
- **721. Porta estreita** — `Mt 7:13-14`
- **722. Falsos profetas** — `Mt 7:15-20`
- **723. Senhor Senhor** — `Mt 7:21-23`
- **724. Casa sobre a rocha** — `Mt 7:24-27`
- **725. Maior mandamento** — `Mt 22:37-38`
- **726. Segundo mandamento** — `Mt 22:39`
- **727. Sábado no ensino de Jesus** — `Mc 2:27-28`
- **728. Pureza do coração** — `Mc 7:14-23`
- **729. Humildade no ensino de Jesus** — `Mt 18:1-5`
- **730. Perdão entre irmãos** — `Mt 18:21-35`
- **731. Servo como grande** — `Mc 10:42-45`
- **732. Riqueza** — `Mc 10:17-27`
- **733. Tributo a César** — `Mt 22:15-22`
- **734. Ressurreição dos mortos no debate com saduceus** — `Mt 22:23-33`

### Bloco Z — Parábolas

*Objetivo do bloco:* Dar a cada parábola uma unidade de estudo própria.

- **735. Parábola do semeador** — `Mt 13:1-23`
- **736. Parábola do joio** — `Mt 13:24-30`
- **737. Parábola do grão de mostarda** — `Mt 13:31-32`
- **738. Parábola do fermento** — `Mt 13:33`
- **739. Parábola do tesouro escondido** — `Mt 13:44`
- **740. Parábola da pérola** — `Mt 13:45-46`
- **741. Parábola da rede** — `Mt 13:47-50`
- **742. Parábola do servo impiedoso** — `Mt 18:23-35`
- **743. Parábola dos trabalhadores da vinha** — `Mt 20:1-16`
- **744. Parábola dos dois filhos** — `Mt 21:28-32`
- **745. Parábola dos lavradores maus** — `Mt 21:33-46`
- **746. Parábola das bodas** — `Mt 22:1-14`
- **747. Parábola das dez virgens** — `Mt 25:1-13`
- **748. Parábola dos talentos** — `Mt 25:14-30`
- **749. Parábola da ovelha perdida** — `Lc 15:3-7`
- **750. Parábola da moeda perdida** — `Lc 15:8-10`
- **751. Parábola do filho perdido** — `Lc 15:11-32`
- **752. Parábola do bom samaritano** — `Lc 10:25-37`
- **753. Parábola do amigo à meia-noite** — `Lc 11:5-8`
- **754. Parábola do rico insensato** — `Lc 12:13-21`
- **755. Parábola dos servos vigilantes** — `Lc 12:35-40`
- **756. Parábola do administrador fiel** — `Lc 12:42-48`
- **757. Parábola da figueira estéril** — `Lc 13:6-9`
- **758. Parábola do grande banquete** — `Lc 14:15-24`
- **759. Parábola do administrador injusto** — `Lc 16:1-13`
- **760. Parábola do rico e Lázaro** — `Lc 16:19-31`
- **761. Parábola do juiz injusto** — `Lc 18:1-8`
- **762. Parábola do fariseu e publicano** — `Lc 18:9-14`
- **763. Parábola das minas** — `Lc 19:11-27`
- **764. Parábola da semente que cresce** — `Mc 4:26-29`

### Bloco AA — Sinais e milagres

*Objetivo do bloco:* Investigar cada sinal como narrativa própria, antes de qualquer síntese temática.

- **765. Água em vinho** — `Jo 2:1-11`
- **766. Cura do filho do oficial** — `Jo 4:46-54`
- **767. Pesca maravilhosa em Lucas 5** — `Lc 5:1-11`
- **768. Endemoninhado de Cafarnaum** — `Mc 1:21-28`
- **769. Sogra de Pedro** — `Mc 1:29-31`
- **770. Purificação do leproso** — `Mc 1:40-45`
- **771. Paralítico de Cafarnaum** — `Mc 2:1-12`
- **772. Homem da mão ressequida** — `Mc 3:1-6`
- **773. Servo do centurião** — `Mt 8:5-13`
- **774. Filho da viúva de Naim** — `Lc 7:11-17`
- **775. Tempestade acalmada** — `Mc 4:35-41`
- **776. Endemoninhado geraseno** — `Mc 5:1-20`
- **777. Mulher com hemorragia** — `Mc 5:25-34`
- **778. Filha de Jairo** — `Mc 5:21-43`
- **779. Dois cegos** — `Mt 9:27-31`
- **780. Mudo endemoninhado** — `Mt 9:32-34`
- **781. Multiplicação dos cinco mil** — `Mc 6:30-44`
- **782. Jesus andando sobre o mar** — `Mt 14:22-33`
- **783. Filha da mulher siro-fenícia** — `Mc 7:24-30`
- **784. Surdo gago** — `Mc 7:31-37`
- **785. Multiplicação dos quatro mil** — `Mc 8:1-10`
- **786. Cego de Betsaida** — `Mc 8:22-26`
- **787. Menino com espírito impuro** — `Mc 9:14-29`
- **788. Moeda na boca do peixe** — `Mt 17:24-27`
- **789. Dez leprosos** — `Lc 17:11-19`
- **790. Cego de nascença** — `Jo 9`
- **791. Lázaro** — `Jo 11`
- **792. Cego Bartimeu** — `Mc 10:46-52`
- **793. Figueira seca** — `Mc 11:12-25`
- **794. Orelha de Malco** — `Lc 22:50-51`
- **795. Pesca de João 21** — `Jo 21:1-14`

### Bloco AB — Conflito e paixão

*Objetivo do bloco:* Percorrer cada etapa final de Jesus como estudo separado.

- **796. Confissão de Pedro** — `Mt 16:13-20`
- **797. Primeiro anúncio da paixão** — `Mt 16:21`
- **798. Transfiguração** — `Mt 17:1-8`
- **799. Entrada em Jerusalém** — `Mt 21:1-11`
- **800. Purificação do templo** — `Mt 21:12-17`
- **801. Unção em Betânia** — `Jo 12:1-8`
- **802. Conspiração para matar Jesus** — `Mt 26:1-5`
- **803. Traição de Judas** — `Mt 26:14-16`
- **804. Última ceia** — `Mt 26:17-30`
- **805. Pão na instituição da ceia** — `Mt 26:26`
- **806. Cálice na instituição da ceia** — `Mt 26:27-29`
- **807. Nova aliança no sangue** — `Lc 22:20`
- **808. Lava-pés** — `Jo 13`
- **809. Novo mandamento** — `Jo 13:34`
- **810. Promessa do Consolador** — `Jo 14:16`
- **811. Oração sacerdotal** — `Jo 17`
- **812. Getsêmani** — `Mt 26:36-46`
- **813. Prisão de Jesus** — `Mt 26:47-56`
- **814. Audiência diante do sumo sacerdote** — `Mt 26:57-68`
- **815. Negação de Pedro** — `Mt 26:69-75`
- **816. Julgamento diante de Pilatos** — `Jo 18:28–19:16`
- **817. Barrabás** — `Mt 27:15-26`
- **818. Flagelação** — `Jo 19:1`
- **819. Coroa de espinhos** — `Jo 19:2`
- **820. Crucificação** — `Jo 19:16-37`
- **821. Sete palavras da cruz como conjunto textual** — `Mt 27; Mc 15; Lc 23; Jo 19`
- **822. Trevas na crucificação** — `Mt 27:45`
- **823. Véu rasgado** — `Mt 27:51`
- **824. Lado traspassado** — `Jo 19:34`
- **825. Sepultamento** — `Jo 19:38-42`

### Bloco AC — Ressurreição e ascensão

*Objetivo do bloco:* Investigar a sequência pós-cruz sem condensar testemunhos.

- **826. Túmulo vazio** — `Mt 28; Mc 16; Lc 24; Jo 20`
- **827. Mulheres no túmulo** — `Mt 28:1-10`
- **828. Maria Madalena** — `Jo 20:11-18`
- **829. Pedro no túmulo** — `Lc 24:12`
- **830. Discípulos de Emaús** — `Lc 24:13-35`
- **831. Aparição aos discípulos** — `Lc 24:36-49`
- **832. Tomé** — `Jo 20:24-29`
- **833. Aparição na Galileia** — `Mt 28:16-20`
- **834. Grande comissão** — `Mt 28:18-20`
- **835. Aparição junto ao mar** — `Jo 21`
- **836. Restauração de Pedro** — `Jo 21:15-19`
- **837. Quarenta dias** — `At 1:3`
- **838. Ascensão** — `At 1:9`
- **839. Nuvem na ascensão** — `At 1:9`
- **840. Promessa do retorno** — `At 1:10-11`
- **841. Sessão à direita de Deus** — `At 2:33-36`
- **842. Testemunho apostólico da ressurreição** — `At 2–4`
- **843. Ressurreição em 1 Coríntios 15** — `1Co 15`
- **844. Primícias dos que dormem** — `1Co 15:20`
- **845. Corpo ressurreto** — `1Co 15:35-49`

### Bloco AD — Atos e Espírito

*Objetivo do bloco:* Seguir a expansão da missão apostólica por temas isolados.

- **846. Escolha de Matias** — `At 1:15-26`
- **847. Pentecostes** — `At 2`
- **848. Línguas em Atos 2** — `At 2:1-13`
- **849. Sermão de Pedro em Atos 2** — `At 2:14-41`
- **850. Comunidade de Atos 2** — `At 2:42-47`
- **851. Cura do coxo** — `At 3`
- **852. Oposição do Sinédrio** — `At 4`
- **853. Ananias e Safira** — `At 5`
- **854. Sete servidores** — `At 6`
- **855. Estêvão** — `At 6–7`
- **856. Martírio de Estêvão** — `At 7`
- **857. Filipe em Samaria** — `At 8`
- **858. Eunuco etíope** — `At 8:26-40`
- **859. Conversão de Saulo** — `At 9`
- **860. Cornélio** — `At 10`
- **861. Gentios recebem o Espírito** — `At 10:44-48`
- **862. Igreja em Antioquia** — `At 11:19-26`
- **863. Primeira viagem de Paulo** — `At 13–14`
- **864. Questão da circuncisão em Atos 15** — `At 15`
- **865. Segunda viagem de Paulo** — `At 15:36–18:22`
- **866. Terceira viagem de Paulo** — `At 18:23–21:17`
- **867. Paulo em Jerusalém** — `At 21–23`
- **868. Paulo diante de Félix** — `At 24`
- **869. Paulo diante de Festo** — `At 25`
- **870. Paulo diante de Agripa** — `At 26`
- **871. Naufrágio** — `At 27`
- **872. Paulo em Roma** — `At 28`

### Bloco AE — Salvação

*Objetivo do bloco:* Construir a linguagem soteriológica diretamente dos textos apostólicos.

- **873. Pecado universal** — `Rm 3:23`
- **874. Salário do pecado** — `Rm 6:23`
- **875. Ira de Deus** — `Rm 1:18`
- **876. Graça** — `Ef 2:8`
- **877. Fé** — `Rm 3:28`
- **878. Arrependimento** — `At 17:30`
- **879. Justificação** — `Rm 3–5`
- **880. Justiça de Deus** — `Rm 3:21-26`
- **881. Propiciação** — `Rm 3:25`
- **882. Redenção** — `Rm 3:24`
- **883. Reconciliação** — `2Co 5:18-21`
- **884. Substituição** — `2Co 5:21`
- **885. Expiação** — `Hb 9`
- **886. Perdão como resultado da redenção** — `Ef 1:7`
- **887. Novo nascimento em 1 Pedro** — `1Pe 1:23`
- **888. Regeneração** — `Tt 3:5`
- **889. Adoção** — `Rm 8:15`
- **890. Santificação** — `1Ts 4:3`
- **891. Glorificação** — `Rm 8:30`
- **892. União com Cristo** — `Rm 6`
- **893. Morte com Cristo** — `Rm 6:3-8`
- **894. Ressurreição com Cristo** — `Cl 3:1`
- **895. Nova criação em 2 Coríntios 5** — `2Co 5:17`
- **896. Vida eterna** — `Jo 3:16`
- **897. Segurança em Cristo** — `Rm 8:31-39`
- **898. Perseverança** — `Hb 10:36`
- **899. Apostasia como advertência** — `Hb 6`
- **900. Obras e fé em Tiago** — `Tg 2:14-26`
- **901. Lei da fé em Romanos** — `Rm 3:27`
- **902. Eleição em Efésios 1** — `Ef 1:3-14`
- **903. Predestinação em Romanos 8** — `Rm 8:28-30`
- **904. Chamado** — `Rm 8:30`
- **905. Consciência** — `Rm 2:15`
- **906. Juízo segundo obras** — `Rm 2:6`
- **907. Salvação dos gentios** — `Rm 11`
- **908. Israel em Romanos 9–11** — `Rm 9–11`

### Bloco AF — Espírito Santo

*Objetivo do bloco:* Dar ao tema do Espírito uma trilha própria e textual.

- **909. Espírito na criação** — `Gn 1:2`
- **910. Espírito sobre líderes de Israel** — `Nm 11:25`
- **911. Espírito sobre juízes** — `Jz 3:10`
- **912. Espírito sobre Davi** — `1Sm 16:13`
- **913. Espírito nos profetas** — `Ez 2:2`
- **914. Promessa de Joel** — `Jl 2:28-32`
- **915. Espírito no nascimento de Jesus** — `Lc 1:35`
- **916. Espírito no batismo de Jesus** — `Lc 3:22`
- **917. Espírito no ministério de Jesus** — `Lc 4:18`
- **918. Consolador** — `Jo 14:16`
- **919. Espírito da verdade** — `Jo 14:17`
- **920. Espírito ensina** — `Jo 14:26`
- **921. Espírito testemunha de Cristo** — `Jo 15:26`
- **922. Espírito convence** — `Jo 16:8`
- **923. Espírito guia** — `Jo 16:13`
- **924. Pentecostes e Espírito** — `At 2`
- **925. Dom do Espírito** — `At 2:38`
- **926. Batismo no Espírito** — `1Co 12:13`
- **927. Habitação do Espírito** — `Rm 8:9`
- **928. Templo do Espírito** — `1Co 6:19`
- **929. Selo do Espírito** — `Ef 1:13`
- **930. Penhor do Espírito** — `Ef 1:14`
- **931. Fruto do Espírito** — `Gl 5:22-23`
- **932. Dons do Espírito** — `1Co 12`
- **933. Andar no Espírito** — `Gl 5:16`
- **934. Não entristecer o Espírito** — `Ef 4:30`
- **935. Não apagar o Espírito** — `1Ts 5:19`
- **936. Intercessão do Espírito** — `Rm 8:26`
- **937. Espírito e ressurreição** — `Rm 8:11`
- **938. Blasfêmia contra o Espírito** — `Mc 3:28-30`

### Bloco AG — Igreja

*Objetivo do bloco:* Construir a eclesiologia por elementos textuais separados.

- **939. Significado de ekklesia** — `Mt 16:18`
- **940. Cristo como cabeça** — `Cl 1:18`
- **941. Igreja como corpo** — `1Co 12:27`
- **942. Igreja como templo** — `Ef 2:21-22`
- **943. Igreja como noiva** — `Ef 5:25-32`
- **944. Pedras vivas** — `1Pe 2:5`
- **945. Sacerdócio santo** — `1Pe 2:5`
- **946. Batismo** — `Rm 6:3-4`
- **947. Batismo em Atos** — `At 2:38-41`
- **948. Ceia do Senhor** — `1Co 11:23-26`
- **949. Pão na comunhão da ceia** — `1Co 10:16`
- **950. Cálice na comunhão da ceia** — `1Co 10:16`
- **951. Unidade** — `Ef 4:1-6`
- **952. Disciplina na igreja** — `Mt 18:15-20`
- **953. Restauração do pecador** — `Gl 6:1`
- **954. Presbíteros** — `1Tm 3; Tt 1`
- **955. Diáconos** — `1Tm 3:8-13`
- **956. Pastores como liderança da igreja** — `Ef 4:11`
- **957. Mestres** — `Ef 4:11`
- **958. Evangelistas** — `Ef 4:11`
- **959. Apóstolos** — `Ef 4:11`
- **960. Profetas** — `Ef 4:11`
- **961. Diversidade de dons** — `1Co 12`
- **962. Amor como caminho superior** — `1Co 13`
- **963. Ordem na reunião** — `1Co 14`
- **964. Cântico congregacional** — `Ef 5:19`
- **965. Oração congregacional** — `At 4:24-31`
- **966. Oferta para necessitados** — `2Co 8–9`
- **967. Missão** — `Mt 28:18-20`
- **968. Envio** — `At 13:1-3`
- **969. Hospitalidade como prática comunitária** — `Rm 12:13`
- **970. Viúvas** — `1Tm 5`
- **971. Órfãos** — `Tg 1:27`
- **972. Pobres** — `Tg 2`
- **973. Perseguição da igreja** — `At 8:1`
- **974. Falsos mestres** — `2Pe 2`
- **975. Teste dos espíritos** — `1Jo 4:1`
- **976. Cartas às sete igrejas como exame eclesial** — `Ap 2–3`

### Bloco AH — Vida cristã

*Objetivo do bloco:* Estudar ética e prática com um tema por unidade.

- **977. Amor a Deus** — `Mt 22:37`
- **978. Amor ao próximo** — `Mt 22:39`
- **979. Amor aos inimigos** — `Mt 5:44`
- **980. Perdão mútuo em Colossenses** — `Cl 3:13`
- **981. Misericórdia** — `Lc 6:36`
- **982. Justiça** — `Mq 6:8`
- **983. Humildade em Filipenses 2** — `Fp 2:3`
- **984. Mansidão** — `Gl 5:23`
- **985. Paciência** — `Tg 5:7`
- **986. Bondade** — `Gl 5:22`
- **987. Fidelidade** — `Gl 5:22`
- **988. Domínio próprio** — `Gl 5:23`
- **989. Alegria** — `Fp 4:4`
- **990. Paz** — `Fp 4:6-7`
- **991. Ansiedade em Filipenses** — `Fp 4:6`
- **992. Oração** — `1Ts 5:17`
- **993. Jejum** — `Mt 6:16-18`
- **994. Generosidade** — `2Co 9:7`
- **995. Dinheiro** — `1Tm 6:10`
- **996. Contentamento** — `Fp 4:11-13`
- **997. Trabalho** — `Cl 3:23`
- **998. Descanso** — `Hb 4`
- **999. Fala** — `Ef 4:29`
- **1000. Mentira** — `Ef 4:25`
- **1001. Ira na vida cristã** — `Ef 4:26`
- **1002. Roubo** — `Ef 4:28`
- **1003. Embriaguez** — `Ef 5:18`
- **1004. Sexualidade** — `1Co 6:12-20`
- **1005. Fornicação** — `1Ts 4:3`
- **1006. Adultério** — `Hb 13:4`
- **1007. Casamento** — `Ef 5:22-33`
- **1008. Solteirice** — `1Co 7`
- **1009. Divórcio na instrução apostólica** — `1Co 7; Mt 19`
- **1010. Pais** — `Ef 6:4`
- **1011. Filhos** — `Ef 6:1-3`
- **1012. Viúvez** — `1Tm 5`
- **1013. Amizade segundo Jesus** — `Jo 15:13-15`
- **1014. Hospitalidade ao estrangeiro** — `Hb 13:2`
- **1015. Governo civil** — `Rm 13:1-7`
- **1016. Obediência a Deus diante do Estado** — `At 5:29`
- **1017. Justiça para o pobre** — `Tg 2`
- **1018. Cuidado do estrangeiro** — `Hb 13:2`
- **1019. Cuidado do enfermo** — `Mt 25:36`
- **1020. Prisão** — `Mt 25:36`
- **1021. Sofrimento** — `1Pe`
- **1022. Perseguição** — `Mt 5:10-12`
- **1023. Disciplina de Deus** — `Hb 12:5-11`
- **1024. Tentação** — `Tg 1:12-15`
- **1025. Confissão de pecados** — `1Jo 1:9`
- **1026. Comunhão** — `1Jo 1:7`
- **1027. Consciência fraca** — `Rm 14`
- **1028. Liberdade cristã** — `Gl 5:1`
- **1029. Tropeço do irmão** — `1Co 8`
- **1030. Comida sacrificada a ídolos** — `1Co 8–10`
- **1031. Vingança** — `Rm 12:19`
- **1032. Inimigos** — `Rm 12:20`
- **1033. Bênção aos perseguidores** — `Rm 12:14`

### Bloco AI — Esperança futura

*Objetivo do bloco:* Organizar escatologia por afirmações distintas antes de sistemas interpretativos.

- **1034. Morte física** — `Hb 9:27`
- **1035. Estado dos mortos**
- **1036. Ressurreição dos justos** — `Jo 5:29`
- **1037. Ressurreição dos injustos** — `Jo 5:29`
- **1038. Corpo incorruptível** — `1Co 15:52-54`
- **1039. Volta de Jesus** — `At 1:11`
- **1040. Parousia** — `1Ts 4:15`
- **1041. Sinal do Filho do Homem** — `Mt 24:30`
- **1042. Vigilância** — `Mt 24:42`
- **1043. Dia do Senhor** — `1Ts 5:2`
- **1044. Homem da iniquidade** — `2Ts 2`
- **1045. Apostasia em 2 Tessalonicenses** — `2Ts 2:3`
- **1046. Ressurreição em 1 Tessalonicenses 4** — `1Ts 4:13-18`
- **1047. Encontro com o Senhor** — `1Ts 4:17`
- **1048. Transformação dos vivos** — `1Co 15:51-52`
- **1049. Tribunal de Cristo** — `2Co 5:10`
- **1050. Juízo final** — `Ap 20:11-15`
- **1051. Livro da vida** — `Ap 20:12,15`
- **1052. Segunda morte** — `Ap 20:14`
- **1053. Geena** — `Mt 10:28`
- **1054. Vida eterna futura** — `Mt 25:46`
- **1055. Novo céu** — `Ap 21:1`
- **1056. Nova terra** — `Ap 21:1`
- **1057. Nova Jerusalém** — `Ap 21:2`
- **1058. Deus habitando com os homens** — `Ap 21:3`
- **1059. Fim da morte** — `Ap 21:4`
- **1060. Fim do luto** — `Ap 21:4`
- **1061. Fim da dor** — `Ap 21:4`
- **1062. Rio da vida** — `Ap 22:1`
- **1063. Árvore da vida na esperança futura** — `Ap 22:2`

### Bloco AJ — Apocalipse

*Objetivo do bloco:* Ler o último livro em unidades próprias sem impor previamente um sistema escatológico.

- **1064. Prólogo de Apocalipse** — `Ap 1:1-3`
- **1065. Testemunho de Jesus em Apocalipse** — `Ap 1:2`
- **1066. Bem-aventurança da leitura** — `Ap 1:3`
- **1067. Visão do Cristo glorificado** — `Ap 1:9-20`
- **1068. Éfeso** — `Ap 2:1-7`
- **1069. Esmirna** — `Ap 2:8-11`
- **1070. Pérgamo** — `Ap 2:12-17`
- **1071. Tiatira** — `Ap 2:18-29`
- **1072. Sardes** — `Ap 3:1-6`
- **1073. Filadélfia** — `Ap 3:7-13`
- **1074. Laodiceia** — `Ap 3:14-22`
- **1075. Trono celestial** — `Ap 4`
- **1076. Cordeiro e o livro** — `Ap 5`
- **1077. Primeiro selo** — `Ap 6:1-2`
- **1078. Segundo selo** — `Ap 6:3-4`
- **1079. Terceiro selo** — `Ap 6:5-6`
- **1080. Quarto selo** — `Ap 6:7-8`
- **1081. Quinto selo** — `Ap 6:9-11`
- **1082. Sexto selo** — `Ap 6:12-17`
- **1083. Cento e quarenta e quatro mil** — `Ap 7:1-8`
- **1084. Grande multidão** — `Ap 7:9-17`
- **1085. Sétimo selo** — `Ap 8:1`
- **1086. Primeira trombeta** — `Ap 8:7`
- **1087. Segunda trombeta** — `Ap 8:8-9`
- **1088. Terceira trombeta** — `Ap 8:10-11`
- **1089. Quarta trombeta** — `Ap 8:12`
- **1090. Quinta trombeta** — `Ap 9:1-12`
- **1091. Sexta trombeta** — `Ap 9:13-21`
- **1092. Livrinho** — `Ap 10`
- **1093. Duas testemunhas** — `Ap 11`
- **1094. Sétima trombeta** — `Ap 11:15-19`
- **1095. Mulher de Apocalipse 12** — `Ap 12`
- **1096. Dragão** — `Ap 12`
- **1097. Besta do mar** — `Ap 13:1-10`
- **1098. Besta da terra** — `Ap 13:11-18`
- **1099. Marca da besta** — `Ap 13:16-18`
- **1100. Cordeiro no monte Sião** — `Ap 14:1-5`
- **1101. Três anjos** — `Ap 14:6-13`
- **1102. Ceifa da terra** — `Ap 14:14-20`
- **1103. Sete taças** — `Ap 15–16`
- **1104. Babilônia** — `Ap 17–18`
- **1105. Bodas do Cordeiro** — `Ap 19:6-10`
- **1106. Cavaleiro fiel e verdadeiro** — `Ap 19:11-21`
- **1107. Mil anos** — `Ap 20:1-6`
- **1108. Derrota final de Satanás** — `Ap 20:7-10`
- **1109. Grande trono branco** — `Ap 20:11-15`
- **1110. Nova criação em Apocalipse 21** — `Ap 21:1-8`
- **1111. Cidade santa** — `Ap 21:9-27`
- **1112. Rio da água da vida** — `Ap 22:1`
- **1113. Árvore da vida em Apocalipse 22** — `Ap 22:2`
- **1114. Servos verão o rosto de Deus** — `Ap 22:4`
- **1115. Jesus vem sem demora** — `Ap 22:7,12,20`
- **1116. Convite final** — `Ap 22:17`
- **1117. Advertência final** — `Ap 22:18-19`
- **1118. Graça final** — `Ap 22:21`

## 6. Estrutura de dados proposta

```js
{
  id: "estudo-001",
  theme: "O que é uma afirmação testável",
  block: "A",
  prerequisites: [],
  scripture: [],
  claims: [],
  references: [],
  observations: [],
  inferences: [],
  limits: [],
  status: "planned"
}
```

Uma `reference` nunca contém somente `url`. Ela aponta para um objeto interno:

```js
{
  id: "pilate-stone",
  kind: "inscription",
  viewer: "InscriptionViewer",
  localAssets: [],
  transcription: [],
  metadata: {},
  source: { owner: "...", officialUrl: "...", checkedAt: "..." },
  license: {},
  demonstrates: [],
  doesNotDemonstrate: []
}
```

## 7. Estado técnico/editorial e próximos gates

### v0.2 — Arquitetura — concluído
- trilha de 1118 estudos atômicos definida;
- apoio corrigido;
- referência interna especificada;
- catálogo messiânico preservado;
- UX formalizada como gate de aceite.

### v0.3 — Corpus executável — concluído nesta entrega
- currículo e dados editoriais separados do HTML;
- 1118 estudos estruturados e navegáveis;
- roteamento por estudo;
- busca e filtros da trilha;
- progresso local;
- painel universal de referência;
- leitor bíblico interno reutilizável;
- tradução → original → estudo do original;
- registro interno de fontes materiais/textuais;
- relações internas e sequência entre estudos;
- preservação do módulo de 357 relações messiânicas.

### Gate seguinte — auditoria de profundidade
- revisar referências bíblicas unidade por unidade;
- aumentar o número de relações internas explícitas onde o corpus exigir;
- ampliar glossários hebraico/aramaico/grego sem transformar léxico em interpretação;
- incorporar fac-símiles/imagens apenas quando licença e proveniência permitirem;
- revisar cada fonte material contra o catálogo custodiante mais direto disponível;
- registrar variantes textuais relevantes com testemunhos lado a lado;
- testar navegação, foco, histórico, leitura longa e desempenho em celulares reais.

### v1.0 — Auditoria integral
- nenhum estudo sem referências internas navegáveis quando houver texto-base;
- nenhuma conclusão doutrinária dependente de autoridade externa;
- nenhuma evidência essencial reduzida a hyperlink;
- licenças e proveniência auditadas;
- acessibilidade, mobile, performance e coerência auditados;
- trilha termina em Apocalipse 22:21.

## 8. Checklist obrigatório por estudo

- [ ] Tema realmente único.
- [ ] Pré-requisitos explícitos.
- [ ] Texto-base disponível dentro do site.
- [ ] Contexto imediato acessível sem sair do estudo.
- [ ] Original acessível sob demanda.
- [ ] Relações internas navegáveis.
- [ ] Fonte externa primária quando aplicável.
- [ ] Fonte examinável dentro do site.
- [ ] Link oficial disponível como auditoria.
- [ ] Licença/proveniência registradas.
- [ ] Observação separada de inferência.
- [ ] Limites declarados.
- [ ] Sem credo/comentarista como autoridade.
- [ ] Funciona com botão voltar.
- [ ] Funciona em tela estreita.
- [ ] Foco retorna ao ponto de origem.
- [ ] Reduced motion respeitado.
- [ ] Sem erro JS.
- [ ] Sem bloqueio por rede para conteúdo essencial já empacotado.
- [ ] Próximo estudo depende somente do que já foi construído.

## 9. Encerramento da trilha

O último estudo é **Graça final — Apocalipse 22:21**. A experiência termina no próprio encerramento do texto:

> Que a graça do Senhor Jesus seja com todos.
