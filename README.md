# 💬 Finora — Assistente de Finanças Pessoais com IA

Projeto desenvolvido para o desafio **Criando um App de Organização de Finanças Pessoais com Vibe Coding**, da [Digital Innovation One](https://www.dio.me/).

A Finora transforma o controle financeiro em uma conversa simples: a pessoa escreve como fala, e o agente interpreta, classifica e registra entradas e despesas, apresenta resumos e oferece orientações sem julgamentos.

[![Aplicação](https://img.shields.io/badge/Acessar%20a%20Finora-21877A?style=for-the-badge&logo=googlechrome&logoColor=white)](https://finora-chat-finance.lovable.app)
[![Código](https://img.shields.io/badge/Código--fonte-GitHub-181717?style=for-the-badge&logo=github)](https://github.com/jessicafmaximiano/finora-chat-finance)

## 🎯 Problema

Muitas pessoas abandonam o controle financeiro porque os aplicativos tradicionais exigem formulários, classificações manuais e interpretação de relatórios complexos. Isso é especialmente difícil para iniciantes, trabalhadores autônomos e pessoas com diferentes fontes de renda.

A proposta da Finora é reduzir essa barreira por meio de uma experiência conversacional, acessível e educativa.

## 👥 Público-alvo

- Pessoas iniciantes em organização financeira;
- Trabalhadores autônomos;
- Pessoas com renda variável ou diferentes fontes de renda;
- Usuários que consideram planilhas e aplicativos tradicionais complicados.

## 📋 Prompt final — PRD

O texto abaixo foi utilizado como briefing principal para orientar a IA durante a concepção e o desenvolvimento da Finora.

```txt
# Contexto

Quero criar um aplicativo chamado Finora, um assistente de organização de finanças pessoais baseado em conversas em linguagem natural.

A proposta é permitir que o usuário organize seu dinheiro escrevendo como fala, sem depender de planilhas, formulários extensos ou relatórios complexos.

# Problema

Muitas pessoas abandonam o controle financeiro porque os aplicativos exigem preenchimento manual, classificação de despesas e conhecimento para interpretar relatórios.

Quero resolver esse problema com uma experiência conversacional simples, capaz de registrar movimentações, organizar informações e explicar a situação financeira em linguagem acessível.

# Público-alvo

Pessoas iniciantes em organização financeira, trabalhadores autônomos e pessoas com diferentes fontes de renda.

# Funcionalidades prioritárias do MVP

1. Registro por linguagem natural:
   interpretar frases como "gastei R$ 35 no mercado" ou "recebi R$ 1.200 de um freela", identificando valor, tipo, descrição e data.

2. Classificação automática:
   classificar transações em categorias como Mercado, Transporte, Moradia, Saúde, Educação, Lazer, Assinaturas, Contas, Dívidas, Renda e Outros, permitindo correção.

3. Visão de saldo:
   apresentar entradas, despesas, saldo e gastos por categoria em linguagem simples.

4. Metas financeiras:
   permitir criar e consultar metas, como "juntar R$ 1.000 para uma viagem", mostrando o progresso.

5. Dicas personalizadas:
   oferecer sugestões curtas baseadas nos dados reais do usuário, sem julgamentos.

# Agente Financeiro

O agente deve:

- conversar sempre em português brasileiro;
- ter tom acolhedor, educativo e objetivo;
- evitar julgamentos sobre escolhas financeiras;
- explicar termos quando necessário;
- confirmar valor, categoria e data após cada registro;
- permitir correções;
- nunca inventar valores;
- utilizar somente dados reais do usuário;
- oferecer no máximo uma dica por vez;
- celebrar pequenos avanços.

# Fluxo esperado

1. Cadastro ou login;
2. Conversa como tela principal;
3. Registro de entradas e despesas;
4. Consulta do resumo financeiro;
5. Criação e acompanhamento de metas;
6. Acesso a configurações e perfil.

# Recursos necessários

- Frontend responsivo em React;
- Banco de dados para perfis, mensagens, transações e metas;
- Autenticação e isolamento de dados por usuário;
- IA para interpretar frases, classificar movimentações e produzir respostas;
- Interface conversacional simples e acessível.

# Regras do MVP

- Sem integração bancária;
- Registros feitos manualmente pela conversa;
- Valores em reais;
- Dados separados por usuário;
- Sem gráficos ou relatórios complexos nesta primeira versão;
- Linguagem simples, inclusiva e sem julgamentos.

# Entregável esperado

Antes da implementação, apresente:

- cinco funcionalidades prioritárias;
- fluxo conceitual das telas;
- comportamento do agente financeiro;
- recursos necessários;
- plano inicial de validação.

Depois, construa um MVP funcional, responsivo e persistente, preservando a identidade visual da Finora.
```

## ✨ Conceito e funcionalidades

A conversa é o centro da experiência. Em vez de preencher vários campos, o usuário pode escrever:

- “Gastei R$ 35 no mercado hoje.”
- “Recebi R$ 1.200 de um freela.”
- “Como está meu mês?”
- “Crie uma meta de R$ 1.000 para uma viagem.”
- “Me dê uma dica de economia.”

O MVP desenvolvido possui:

- cadastro e autenticação;
- login com Google;
- recuperação de senha;
- registro de entradas e despesas em linguagem natural;
- classificação automática;
- correção de categoria;
- resumo do período;
- criação e consulta de metas;
- dicas baseadas nos registros;
- histórico persistente da conversa;
- proteção dos dados por usuário.

## 🧠 Processo de Vibe Coding

O desenvolvimento foi dividido em etapas para aproveitar melhor cada interação com a IA:

1. **Descoberta e PRD:** definição do problema, público e proposta de valor;
2. **MVP:** priorização das cinco funcionalidades essenciais;
3. **Experiência:** definição do fluxo e do comportamento do agente;
4. **Interface:** criação da identidade visual e da conversa principal;
5. **Persistência:** autenticação, banco de dados e separação dos usuários;
6. **Agente:** interpretação de frases, ferramentas financeiras e respostas;
7. **Validação:** testes com entradas, despesas, resumo e dicas;
8. **Publicação:** hospedagem no Lovable e sincronização com o GitHub.

### Prompts incrementais utilizados

Além do PRD principal, utilizei instruções menores e específicas:

- “Crie o fluxo conceitual das telas com base nas funcionalidades listadas.”
- “Defina o comportamento do Agente Financeiro em português brasileiro, com tom acolhedor, educativo e sem julgamentos.”
- “Transforme a interface em um aplicativo com autenticação e dados persistentes.”
- “Implemente o registro de entradas e despesas em linguagem natural, a classificação automática e o resumo mensal.”
- “Preserve a identidade visual e os componentes já criados.”
- “Use dados reais do usuário e nunca invente valores.”

## 🖼️ Evidências do processo

Durante o desenvolvimento, foram registrados:

- planejamento das cinco funcionalidades prioritárias;
- fluxo conceitual das telas;
- comportamento do agente financeiro;
- recursos técnicos e plano de validação;
- construção da autenticação no Lovable;
- testes do chat com entrada, despesa e resumo mensal;
- geração de dica personalizada a partir dos registros.

Os testes funcionais podem ser reproduzidos na [aplicação publicada](https://finora-chat-finance.lovable.app).

## ✅ Testes realizados

Foram utilizadas as seguintes mensagens:

```txt
Gastei R$ 35 no mercado hoje
Recebi R$ 1.200 de um freela
Como está meu mês?
Me dá uma dica de economia
```

O agente:

- registrou a despesa na categoria Mercado;
- registrou a entrada na categoria Renda;
- calculou R$ 1.200,00 em entradas;
- calculou R$ 35,00 em despesas;
- apresentou saldo positivo de R$ 1.165,00;
- gerou uma dica considerando os registros do período.

## 🧪 Plano de validação

1. Testar o aplicativo com 5 a 10 pessoas do público-alvo durante sete dias;
2. Medir frequência de uso, frases não compreendidas e categorias corrigidas;
3. Realizar entrevistas curtas sobre facilidade e motivação;
4. Considerar sucesso inicial se pelo menos 60% registrarem movimentações em quatro ou mais dias;
5. Ajustar o entendimento de frases antes de adicionar novas telas.

## 💭 Reflexão sobre o processo

### O que funcionou bem?

O principal acerto foi dividir um objetivo amplo em instruções menores. Quando defini problema, público, funcionalidades, tom de voz e limitações, as respostas da IA ficaram mais consistentes. Também funcionou bem validar cada etapa antes de solicitar a próxima.

### O que não funcionou como esperado?

O limite de créditos do Lovable interrompeu o desenvolvimento durante a implementação. Isso me obrigou a priorizar melhor os pedidos, evitar alterações vagas e concentrar vários critérios em cada prompt. Também percebi que uma interface visualmente pronta não significa que autenticação, persistência e segurança estejam concluídas.

### O que aprendi sobre conversar com IAs?

Aprendi que a qualidade do resultado depende da clareza do contexto e dos critérios de aceitação. Pedidos como “crie um aplicativo” são muito abertos. Informar o problema, o público, o comportamento esperado, as restrições e como validar cada entrega transforma a IA em uma parceira de desenvolvimento mais eficiente.

Também aprendi a revisar criticamente as respostas, testar os fluxos e corrigir o direcionamento. Vibe Coding não significa aceitar tudo o que a IA produz; significa conduzir a solução por meio de comunicação, experimentação e validação.

## 🚀 Resultado

Embora o desafio solicitasse apenas o conceito, a proposta evoluiu para um MVP funcional.

- **Aplicação:** https://finora-chat-finance.lovable.app
- **Código-fonte:** https://github.com/jessicafmaximiano/finora-chat-finance
- **Tecnologias:** React, TypeScript, TanStack Start, Tailwind CSS, Supabase e Lovable AI Gateway.

## 👩‍💻 Autora

Desenvolvido por **Jéssica Fernanda Maximiano de Souza** durante a trilha **DIO | Codifique o seu futuro global agora**.

- GitHub: [@jessicafmaximiano](https://github.com/jessicafmaximiano)
