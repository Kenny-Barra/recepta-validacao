# Da Hipótese à Evidência: Validando a Recepta

**Projeto:** Recepta – IA de atendimento e agendamento pelo WhatsApp
**Disciplina:** Metodologias Ágeis e Validação de Produtos
**Aluno:** Kennedy Pereira

## 1. Problema, público e oportunidade

**Problema identificado.** Pequenos negócios de serviço com hora marcada, como salões, barbearias, estúdios e clínicas de estética, fazem quase todo o agendamento pelo WhatsApp e de forma manual. Na maioria deles, quem responde o cliente é a mesma pessoa que atende. Com isso, as mensagens ficam sem resposta durante o serviço, o cliente desiste ou procura outro lugar, e o dono passa o intervalo e a noite respondendo conversas.

**Público.** Donos e profissionais autônomos de negócios de serviço com 1 a 5 profissionais, entre 10 e 150 atendimentos por semana, sem recepcionista e usando o WhatsApp como canal principal.

**Oportunidade.** Hoje é possível usar IA generativa para entender mensagens em linguagem natural ("tem horário sábado de manhã pra corte e barba?") e consultar uma agenda, a um custo baixo por conversa. As ferramentas de agenda que existem exigem que o cliente entre num link ou baixe um app. A oportunidade é atender **dentro da conversa de WhatsApp**, onde o cliente já está.

## 2. Hipóteses

Cada hipótese tem uma métrica e um corte definidos **antes** do experimento.

| Tipo | Hipótese | Como medir | Critério de validação |
|---|---|---|---|
| **H1 – Problema** | Donos de pequenos negócios de serviço perdem tempo e clientes porque não conseguem responder o WhatsApp enquanto atendem. | Nota de dor de 1 a 5 e horas por dia gastas respondendo mensagens | Pelo menos **4 de 6** entrevistados com dor ≥ 4 |
| **H2 – Solução** | Esses donos aceitariam que uma IA respondesse e agendasse **sozinha**, sem aprovar cada mensagem. | Pergunta direta + reação ao protótipo | Pelo menos **4 de 6** respondem "sim" |
| **H3 – Valor** | O ganho de tempo e de clientes justifica pagar uma assinatura mensal. | Valor que pagariam + adesão à lista do piloto | Pelo menos **3 de 6** pagariam ≥ R$ 40/mês **e** pelo menos 3 deixam contato para o piloto |

**Hipótese mais arriscada:** H2. Se o dono não confiar na IA para falar com o cliente, o produto, do jeito que foi pensado, não tem uso. Por isso o experimento foi desenhado para testá-la de frente.

## 3. Solução proposta e definição do MVP

**Solução inicial.** A Recepta seria uma "recepcionista virtual" ligada ao WhatsApp Business do negócio. Ela responde dúvidas (preço, endereço, serviços), oferece os horários livres, marca na agenda e envia lembrete ao cliente, sem que o dono precise interromper o atendimento.

**O que NÃO foi construído.** Nenhuma integração real com WhatsApp, IA em produção ou agenda. Construir isso levaria semanas, e ainda não sabíamos se alguém queria.

**MVP de validação.** Uma **landing page com protótipo navegável** que mostra uma conversa simulada entre cliente e Recepta, os benefícios e o preço sugerido (R$ 49/mês), com um formulário de lista de espera. A landing page foi usada como apoio em **entrevistas curtas de problema e solução** e acompanhada de um **formulário estruturado** com as mesmas perguntas para todos os participantes.

## 4. Como a IA foi usada no discovery

A IA (Claude) foi usada como ferramenta de apoio. Ela não substituiu os usuários.

| Etapa | Uso da IA | O que eu decidi |
|---|---|---|
| Explorar oportunidades | Gerou 10 problemas que IA ou automação poderiam resolver para pequenos negócios | Pontuei cada um por dor percebida, facilidade de acesso ao público e viabilidade, e escolhi o agendamento pelo WhatsApp |
| Formular hipóteses | Sugeriu hipóteses de problema, solução e valor e apontou suposições escondidas | Reescrevi com métricas e cortes numéricos e defini H2 como a mais arriscada |
| Roteiro de entrevista | Revisou o roteiro para tirar perguntas que induzem a resposta ("Você não acha que...?") | Troquei por perguntas sobre comportamento passado ("Me conta a última vez que...") |
| Protótipo | Gerou variações de texto para a landing page | Escolhi a versão mais direta e sem jargão técnico |
| Síntese | Agrupou as anotações das entrevistas por afinidade e contou as menções | Revisei os grupos, interpretei os padrões e tomei a decisão final |

**Limite observado.** Antes das entrevistas, perguntei à IA se donos de salão aceitariam um atendente automático. Ela previu boa aceitação. As entrevistas mostraram o contrário (ver a parte prática), o que confirma a regra da disciplina: **a IA ajuda a organizar, mas não valida mercado**.

## 5. Experimento escolhido e critérios de sucesso

**Experimento:** entrevista de 15 a 20 minutos + demonstração da landing page + formulário estruturado, com 6 potenciais usuários de segmentos diferentes de serviço com hora marcada.

**Por que esse experimento.** Ele testa as três hipóteses de uma vez com custo quase zero. A entrevista revela o comportamento atual (H1), a reação ao protótipo mostra a aceitação da IA (H2) e a pergunta de preço junto com o pedido de contato para o piloto mede o compromisso real (H3), que vale mais que um "achei legal".

**Métricas de sucesso:**

- H1: nº de participantes com dor ≥ 4 (meta: 4 de 6)
- H2: nº de participantes que deixariam a IA responder sozinha (meta: 4 de 6)
- H3: nº que pagariam ≥ R$ 40/mês (meta: 3 de 6) e nº que entram no piloto (meta: 3 de 6)
- Sinal extra: problemas citados **espontaneamente** por 3 ou mais participantes

## 6. Critério de decisão definido antes do experimento

| Decisão | Quando aplicar |
|---|---|
| **Perseverar** | H1, H2 e H3 validadas: seguir para construir o MVP funcional como planejado |
| **Ajustar** | H1 e H3 validadas, mas H2 não: o problema e o valor existem, então se mantém o público e se muda **a forma** da solução |
| **Pivotar** | H1 validada, mas H3 não, **ou** H1 só se confirma em outro segmento: mudar o público ou o modelo de valor |
| **Abandonar** | H1 não validada (menos de 3 de 6 com dor ≥ 4): o problema não é forte o suficiente |

## 7. Organização ágil do trabalho

O trabalho foi feito em três ciclos curtos (Construir, Medir, Aprender), com um quadro Kanban (A fazer, Fazendo, Feito):

1. **Ciclo 1 – Discovery:** oportunidades, hipóteses, Lean Canvas, roteiro de entrevista.
2. **Ciclo 2 – Experimento:** landing page, entrevistas e formulário com os 6 participantes.
3. **Ciclo 3 – Aprendizado:** síntese, comparação com as hipóteses e decisão.

Cada ciclo terminou com uma pergunta de revisão: *"O que aprendemos e o que muda no próximo ciclo?"*

## Links do projeto

- **Repositório no GitHub:** https://github.com/Kenny-Barra/recepta-validacao
- **Vídeo Pitch (YouTube):** https://youtu.be/EP8kXIexTGI
