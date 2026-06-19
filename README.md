# 🤿 Minha Imersão Agentes de IA — ONE (Oracle Next Education)

| ![Alura - ONE Oracle Next Education](/docs/scr/img/logo_alura_one.png) |
|:---:|
| Estou dando os primeiros passos na **Imersão Agentes de IA**, uma fase do programa **ONE (Oracle Next Education)**, criado pela Oracle em parceria com a Alura. Em apenas 5 dias, o objetivo é construir meu primeiro agente de Inteligência Artificial aplicado a um problema real — e este repositório vai documentar essa jornada: o que eu aprendi, os desafios que resolvi e o projeto final que vou desenvolver. |
| <div align="center"> <a href="https://cursos.alura.com.br/user/claudiomendonca" target="_blank"> <img src="https://img.shields.io/badge/Alura.com.br-16537E?style=for-the-badge&logo=alura&logoColor=white" alt="Alura" style="margin-bottom: 5px;" /> </a> </div> |

## Sobre o programa ONE

O ONE é um programa de educação e empregabilidade, 100% online e gratuito, com o objetivo social de capacitar pessoas em tecnologia e conectá-las ao mercado de trabalho por meio de empresas parceiras. A jornada completa dura cerca de 12 meses, passando pelas fases de Tech Foundation e Tech Advanced, com mais de 700 horas de conteúdo.

A Imersão Agentes de IA é a porta de entrada dessa jornada: é a partir dela que poderei concorrer a uma vaga nas próximas fases do programa, na etapa de Cursos Tech. Importante lembrar (e já anotei isso para mim): concluir a imersão não garante automaticamente o ingresso nas fases seguintes.

## O que é a Imersão Agentes de IA

* **Duração:** 5 dias (15/06 a 19/06)
* **Formato:** aulas na plataforma da Alura + comunicação oficial pelo Discord
* **Objetivo:** entender os fundamentos de Inteligência Artificial, explorar ferramentas e conceitos na prática, e aplicar tudo isso construindo um agente de IA do início ao fim

## O que estou aprendendo

Ao longo da semana, os temas centrais são:

- Fundamentos de Inteligência Artificial
- Automação com **n8n**
- **RAG** (Retrieval-Augmented Generation)
- Criação de Agentes de IA

## Cronograma

| Evento | Data |
|---|---|
| Live de abertura | 11/06/2026 |
| Aula 01 no ar | 15/06/2026 |
| Aula 02 no ar | 16/06/2026 |
| Aula 03 no ar | 17/06/2026 |
| Mentoria | 18/06/2026 |
| Live de fechamento | 19/06/2026 |
| Aulas disponíveis até | 19/06/2026, 23h59 |

## Instrutores e Instrutoras da Alura nessa imersão

| Nome | Cargo |
|---|---|
| Eric Oliveira | Supervisor de Conteúdo na Alura Latam, especialista em Java e Spring Boot |
| Giovani Polonio Ticianelli | Principal AI Engineer, com forte atuação em Inteligência Artificial aplicada a negócios |
| Guilherme Lima | Tech Educator e professor na Alura e na USP |

## Masterclass: Introdução à IA Agêntica

### Participe e vá mais fundo

Bem-vindo à nossa Master Class ONE | Imersão em Agentes de IA.

O objetivo desta aula é explorar a evolução da Inteligência Artificial e guiar o próximo grande passo: sair das simples instruções de texto (prompts) e mergulhar no mundo dos Agentes de IA. Esta aula foi desenvolvida especialmente para iniciantes que querem construir sistemas inteligentes de forma visual e prática, sem a necessidade de escrever código.

Neste encontro, vou:

- Entender a diferença entre uma IA comum (que apenas responde) e um Agente de IA, capaz de raciocinar, planejar e executar tarefas por conta própria.
- Configurar as ferramentas fundamentais para dar um "cérebro" e uma memória ao agente, criando contas na Cohere e na Railway.
- Criar uma interface de comunicação acessível, desenvolvendo um bot no Telegram para conversar com o agente.
- Preparar o ambiente para construir fluxos automatizados na ferramenta n8n.

> Atenção: não criar conta no n8n antes da indicação exata durante a aula.

Para aquecer antes da aula ou aprofundar os conhecimentos depois:

1. [Enterprise AI: Private, Secure, Customizable | Cohere](https://cohere.com/)
2. [Railway | The all-in-one intelligent cloud provider](https://railway.com/)
3. [Telegram Messenger](https://telegram.org/)

## Aula 01: O Cérebro do Agente - RAG, Embeddings e n8n

### Participe e vá mais fundo

Você aprenderá:

- O que é RAG (Retrieval-Augmented Generation) e como ele funciona na prática.
- Como transformar documentos em conhecimento usando embeddings.
- Como criar um fluxo de ingestão de dados (Load Data Flow).
- Como estruturar um agente com n8n.
- Como permitir que a IA responda com base em um contexto real.

### Print da aula

![Print da Aula 01 - fluxo de ingestão com RAG, embeddings e vector store](/docs/scr/img/aula01-17062026.png)

### O que eu aprendi

Nesta aula, entendi na prática como um agente pode responder com base em conhecimento real, e não apenas em respostas genéricas do modelo. Aprendi a montar um fluxo de ingestão no n8n, buscar um documento externo via HTTP Request, gerar embeddings com a Cohere e armazenar esse conteúdo em uma vector store para consultas futuras.

Links úteis:

- [n8n](https://n8n.io/)
- [Manual do Colaborador e Políticas de Recursos Humanos - CHOCOLATECH](https://raw.githubusercontent.com/ericmonne/chocolatech-imersao/refs/heads/main/Manual%20de%20RH%20ChocolaTech.txt)
- [GitHub com os arquivos de CHOCOLATECH](https://github.com/ericmonne/chocolatech-imersao)

## Aula 02: Memória e Dados - Integração IA com MySQL

### Participe e vá mais fundo

Você aprenderá:

- Diferença entre dados estruturados (SQL) e não estruturados (RAG).
- Como integrar o agente com um banco de dados (MySQL).
- Como personalizar respostas com dados reais do usuário.
- Como usar IA para preencher parâmetros dinamicamente (`$fromAI`).
- Como combinar RAG + SQL para decisões mais assertivas.

### Print da aula

![Print da Aula 02 - agente com memória, vector store e consulta MySQL](/docs/scr/img/aula02-18062026.png)

### O que eu aprendi

Aqui eu aprendi a combinar duas fontes de informação no mesmo agente: a base vetorial para consultas sobre políticas gerais e o MySQL para dados específicos de cada funcionário. Também entendi melhor como a memória da conversa ajuda o agente a manter contexto, pedir o nome completo quando necessário e responder de forma mais personalizada e útil.

Query SQL:

```sql
CREATE TABLE funcionarios (
	id INT AUTO_INCREMENT PRIMARY KEY,
	nome VARCHAR(100) NOT NULL,
	email VARCHAR(150) NOT NULL UNIQUE,
	departamento VARCHAR(100) NOT NULL,
	cargo VARCHAR(100) NOT NULL,
	data_admissao DATE NOT NULL,
	saldo_ferias INT NOT NULL DEFAULT 0,
	banco_horas DECIMAL(5,1) NOT NULL DEFAULT 0,
	regime VARCHAR(20) NOT NULL DEFAULT 'hibrido'
);

INSERT INTO funcionarios (nome, email, departamento, cargo, data_admissao, saldo_ferias, banco_horas, regime) VALUES
('João Silva', 'joao.silva@empresa.com', 'Engenharia', 'Engenheiro de Software', '2022-03-10', 20, 0.0, 'hibrido'),
('Maria Souza', 'maria.souza@empresa.com', 'Recursos Humanos', 'Analista de RH', '2021-05-15', 5, 12.5, 'hibrido'),
('Carlos Oliveira', 'carlos.oliveira@empresa.com', 'Financeiro', 'Analista Financeiro', '2023-01-20', 0, 0.0, 'presencial'),
('Ana Lima', 'ana.lima@empresa.com', 'Marketing', 'Especialista em Marketing', '2020-11-05', 15, -4.0, 'remoto'),
('Pedro Santos', 'pedro.santos@empresa.com', 'Vendas', 'Executivo de Vendas', '2022-08-01', 10, 8.0, 'hibrido'),
('Fernanda Costa', 'fernanda.costa@empresa.com', 'Operações', 'Gerente de Operações', '2019-02-12', 30, 0.0, 'presencial'),
('Rafael Mendes', 'rafael.mendes@empresa.com', 'TI', 'Analista de Suporte', '2023-06-10', 0, 15.5, 'hibrido'),
('Juliana Rocha', 'juliana.rocha@empresa.com', 'Engenharia', 'Desenvolvedora Front-end', '2021-09-25', 12, 0.0, 'remoto'),
('Bruno Alves', 'bruno.alves@empresa.com', 'Design', 'Designer UX/UI', '2022-04-18', 8, 3.5, 'hibrido'),
('Camila Ferreira', 'camila.ferreira@empresa.com', 'Atendimento', 'Analista de Atendimento', '2024-01-05', 0, 0.0, 'hibrido'),
('Eric Monné', 'eric.monne@chocolatech.com', 'Produto', 'Instrutor de Cursos', '2024-01-15', 25, 8.0, 'hibrido');
```

System Prompt do Agente:

```text
Você é o HR Buddy, assistente virtual de RH da ChocolaTech.
REGRAS:

1. Sempre responda em português.
2. Responda APENAS dúvidas relacionadas a RH.

IDENTIFICAÇÃO DO FUNCIONÁRIO:

- Se o usuário não disser quem é, pergunte o nome completo dele logo na primeira mensagem.
- Use a ferramenta MySQL para buscar na tabela funcionarios usando SEMPRE o NOME COMPLETO informado pelo usuário na conversa.
- Se encontrado: use os saldos de férias e banco de horas.
- Se não encontrado: não invente dados pessoais. Responda apenas com base nas políticas gerais de RH do Vector Store.
Use a base de conhecimento para dúvidas gerais.
```

## Aula 03: Produto Real - Agentes com Telegram e Automatização

### Participe e vá mais fundo

Você aprenderá:

- Como conectar o agente ao Telegram.
- Como estruturar um fluxo com webhook e mensagens.
- Como implementar guardrails (filtros inteligentes).
- Como gerenciar memória por usuário (session ID).
- Como levar o agente para o mundo real.

### Print da aula

![Print da Aula 03 - integração do agente com Telegram e automação real](/docs/scr/img/aula03-18062026.png)

### O que eu aprendi

Nesta etapa, consegui enxergar o agente funcionando em um cenário real, com mensagens chegando pelo Telegram e respostas sendo enviadas automaticamente pelo n8n. Aprendi como conectar a interface de conversa ao fluxo do agente, aplicar controles para respostas mais seguras e usar memória por sessão para manter uma experiência consistente para cada usuário.

## Resumo do que eu aprendi

Ao longo da imersão, aprendi a diferença entre usar IA apenas com prompts e construir um agente capaz de consultar informações, lembrar contexto e executar fluxos úteis. Entendi como o RAG ajuda a dar contexto confiável ao agente, como o MySQL permite trazer dados estruturados para respostas personalizadas e como o Telegram transforma esse projeto em uma solução prática para uso no dia a dia. O principal aprendizado foi perceber que um agente de IA ganha valor quando une modelo, memória, dados e automação em um único fluxo.

## O que espero entregar ao final

- Um **agente de IA funcional**, criado por mim
- Um **projeto para o portfólio**
- Experiência prática com ferramentas usadas no mercado
- O **certificado de participação** da Imersão

## Como estou me organizando

- Participando ativamente da comunidade no Discord, que é o canal oficial de comunicação da Imersão
- Evitando acumular conteúdo — assistindo às aulas em dia
- Reservando um tempo fixo na agenda todos os dias para estudar e avançar no projeto
- Usando a hashtag **#ImersaoAgentesIAONE** para compartilhar o progresso nas redes sociais

## Sobre o ONE (Oracle Next Education)

O ONE foi criado pela Oracle e é realizado em parceria com a Alura. É um programa de educação, inclusão e empregabilidade que prepara pessoas para atuarem como desenvolvedoras(es) em início de carreira, conectando-as a empresas parceiras no fim da jornada.

## Links úteis

- [Guia oficial da Imersão (Notion)](https://grupoalura.notion.site/imersao-agentes-ia-one)
- [Página do ONE - Oracle Next Education](https://www.oracle.com/br/education/oracle-next-education/)
- Dúvidas sobre a Imersão: contato-one@alura.com.br

## Certificado e conclusão

![Certificado de participação na Imersão Agentes de IA](/docs/scr/img/certificado_imersao01.png)

Concluir esta imersão foi um passo importante na minha jornada em Inteligência Artificial. Além do certificado de participação, levo comigo uma base prática sobre agentes de IA, automação com n8n, uso de RAG, integração com banco de dados e publicação de uma interface real com Telegram. Este repositório representa não só o resultado final do estudo, mas também a evolução do meu aprendizado ao transformar conceitos novos em um projeto funcional.

---

*Este README será atualizado conforme eu avançar pelos dias da Imersão e construir meu agente de IA.*
