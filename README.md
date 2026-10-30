# Checador de Factualidade (PT-BR) para Deepseek

> Skill de checagem de fatos em português, feito para ser usado no Deepseek web. Analisa alegações, triangula fontes e entrega um veredito baseado em Verdadeiro/Falso/outros.

## Como funciona

Como uma mensagem normal, você manda uma notícia, cola um rumor ou uma alegação, ou algo que possa ser interpretado como tal. O bot entrega, a partir disso:

- **A alegação, como interpretada, em uma linha**
- **Um veredito** entre 6: Verdadeiro, Falso, Meia-verdade, Fora de contexto, Desatualizado, Disputado.
- **Um resumo dos detalhes em um parágrafo**
- **Um corpo mais extenso explicando os detalhes, incluindo informação em disputa**
- **Lista de fontes com data de acesso**

> [!NOTE]
> Você pode escrever qualquer coisa: o bot vai interpretar se deve checar algo, ou se é um pedido de esclarecimento. De qualquer forma, evite desviar do propósito para não atrapalhar o contexto.

## Por que usar isso?

- **Simplicidade:** Apenas coloque uma premissa, e o bot te diz se é verdade ou não, com um resumo rápido do que foi encontrado. Se quiser mais detalhes, é só ler o resto.
- **Factualidade:** O bot prioriza sites focados em checar notícias falsas (com Aos Fatos, Agência Lupa) e sites institucionais do governo, além de fontes acadêmicas. Nenhuma informação é inventada, elas todas são retiradas das fontes.
- **Neutralidade:** Mesmo assim, é tentada depois uma triangulação de fontes diversificadas, e é definida a fonte da informação se possível. O método também é preparado para detectar premissa carregada para evitar vieses.

> [!WARNING]
> **Não leia apenas o veredito.** Rumores são complicados e o veredito é apenas uma palavra. Leia o resumo e, quando em dúvida, os detalhes até as fontes, responda o bot e **questione o resultado.**
>
> O veredito pode variar entre sessões e usos. Use seu próprio senso crítico.

## Como usar

1. Acesse [chat.deepseek.com](https://chat.deepseek.com).
2. Cole [este arquivo](https://raw.githubusercontent.com/taitox/ds-checadordefactualidade/refs/heads/main/ds-checador-de-factualidade-ptbr.md) na **primeira mensagem** e escreva **"Siga as instruções."**
3. Envie, e sua próxima mensagem já pode ser um rumor a ser checado.

## Exemplo de uso

Este exemplo está colado tal e qual como foi enviado (rumor) pelo usuário e entregue (resposta) pelo bot. Nenhuma alteração foi feita se não para formatar o texto para ser ainda mais visualmente fiel ao resultado entregue.

### **Rumor:**
> Getúlio Vargas se vestia de palhaço nas horas vagas?

### **Resposta:**
>1. **Alegação enquadrada**
>
> Getúlio Vargas se vestia de palhaço nas horas vagas.
>
>**Veredito: Falso**
>
>2. **Resumo geral**
>
>É falso porque não há fotografia, documento, ata, correspondência ou testemunho que registre Vargas vestido de palhaço; as fontes descrevem seu lazer com charutos, golfe, chimarrão e trajes informais de gaúcho, e a única menção a palhaço é uma foto em que ele sorri para a palhaçada de outra pessoa.
>
>---
>
>3. **Checagem registrada**
>
>Sem checagem registrada até 30/10/2026, porque nenhum dos seis checadores listados publicou verificação sobre esta alegação específica.
>
>4. **Evidência primária**
>
>Sem fonte primária até 30/10/2026, porque não há fotografia, documento, ata, correspondência ou testemunho que registre Vargas caracterizado de palhaço; o registro iconográfico mais próximo mostra Vargas sorrindo diante da palhaçada do Sr. Barreto Pinto, sem que o próprio Vargas estivesse fantasiado.
>
>5. **Triangulação e diversidade**
>- Triangulação: 3 fontes independentes (CEDAP/UFRGS, Museu da República e Retrospecta), sem byline compartilhada e com origens documentais distintas.
>- Diversidade: 2 vozes institucionais (arquivo acadêmico e museu) e 1 voz não afiliada (blog de curiosidades históricas).
>- Contagem: 3 fontes, sendo 2 institucionais e 1 não afiliada.
>
>6. **O que permanece em disputa**
>- Não está em disputa: a ausência de qualquer registro de Vargas vestido de palhaço.
>- Permanece em disputa: nada, a alegação não tem base documental.
>
>7. **Fontes recomendadas**
>- CEDAP/UFRGS — “Um Documento Histórico” (1957-03-18; publicado em 2025-03-28): https://cedap.ufrgs.br/xmlui/handle/20.500.11959/7913?locale-attribute=pt_BR
>- Museu da República — “Fotografias de Getúlio Vargas em residências” (s.d.): https://atom-museurepublica.museus.gov.br/index.php/getulio-vargas-sentado-a-mesa-durante-uma-refeicao-em-uma-residencia
>- Retrospecta — “Curiosidades sobre a Era Vargas” (2017-09-25): https://retrospecta.wordpress.com/2017/09/25/curiosidades-sobre-a-era-vargas/
>
>Deepseek - Checagem de factualidade em: 30/10/2026</summary>
