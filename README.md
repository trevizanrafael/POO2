# README - Sistema de Gestão de Academias GymFlow

[cite_start]Este documento fornece uma visão geral detalhada do sistema GymFlow, um software de gestão para academias[cite: 2]. Ele descreve os objetivos do sistema, os diferentes tipos de usuários, e os requisitos funcionais e não funcionais.

## 1. Visão Geral do Sistema

[cite_start]O GymFlow é um sistema de gestão projetado para centralizar e otimizar os processos administrativos e operacionais de uma academia[cite: 15]. [cite_start]O objetivo principal é automatizar tarefas rotineiras, como o controle de alunos, a gestão financeira e a criação de treinos, permitindo que a equipe se concentre em oferecer um serviço de maior qualidade aos alunos[cite: 16]. [cite_start]A implementação deste sistema visa transformar operações manuais em um fluxo de trabalho digital e eficiente [cite: 17][cite_start], buscando otimizar o tempo da equipe e melhorar a retenção de alunos através de um acompanhamento personalizado[cite: 29, 30].

[cite_start]O sistema foi projetado para atender às necessidades de três tipos de usuários[cite: 18]:

* [cite_start]**Administrador:** Ferramenta para gerenciar cadastros de alunos, instrutores, planos e academias[cite: 19].
* [cite_start]**Instrutor:** Ferramenta de produtividade para cadastrar fichas de treino, acompanhar a evolução dos alunos por meio de avaliações físicas e personalizar os exercícios[cite: 20, 21].
* [cite_start]**Aluno:** Acesso fácil à sua ficha de treino, histórico de pagamentos e acompanhamento de seu progresso através dos resultados das avaliações físicas[cite: 22].

## 2. Requisitos Funcionais

A seguir estão detalhados os requisitos funcionais do sistema, categorizados por perfil de usuário.

### 2.1. Requisitos do Aluno

| Identificador | Descrição | Prioridade |
| :--- | :--- | :--- |
| RF01 | [cite_start]O sistema deve permitir que o Aluno faça login com usuário e senha válidos[cite: 37]. | [cite_start]ALTA [cite: 37] |
| RF02 | [cite_start]O sistema deve exibir mensagem de erro quando o login do Aluno for inválido[cite: 37]. | [cite_start]ALTA [cite: 37] |
| RF03 | [cite_start]O sistema deve permitir que o Aluno visualize sua Ficha de Treino atual, contendo exercícios, peso, repetições e séries[cite: 37]. | [cite_start]ALTA [cite: 37] |
| RF04 | [cite_start]O sistema deve permitir que o Aluno visualize o nome de seu Instrutor responsável[cite: 37]. | [cite_start]ALTA [cite: 37] |
| RF05 | [cite_start]O sistema deve permitir que o Aluno visualize seu Plano de Treino e a Academia onde está cadastrado[cite: 37]. | [cite_start]MÉDIA [cite: 37] |
| RF06 | [cite_start]O sistema deve permitir que o Aluno visualize o histórico de Fichas de Treino anteriores[cite: 37]. | [cite_start]MÉDIA [cite: 37] |
| RF07 | [cite_start]O sistema deve permitir que o Aluno visualize os resultados de Avaliações Físicas (coeficiente de força, gordura corporal, peso e data)[cite: 37]. | [cite_start]MÉDIA [cite: 37] |
| RF08 | [cite_start]O sistema deve permitir que o Aluno consulte o histórico de Avaliações Físicas antigas[cite: 37]. | [cite_start]MÉDIA [cite: 37] |
| RF09 | [cite_start]O sistema deve permitir que o Aluno saia da aplicação (logout)[cite: 37]. | [cite_start]ALTA [cite: 37] |
| RF10 | [cite_start]O sistema deve permitir que o Aluno navegue entre telas (voltar às opções anteriores)[cite: 37]. | [cite_start]ALTA [cite: 37] |
| RF11 | [cite_start]O sistema deve numerar e organizar as fichas de treino do Aluno de forma sequencial (ex.: Treino 1, Treino 2...)[cite: 37]. | [cite_start]BAIXA [cite: 37] |
| RF12 | [cite_start]O sistema deve permitir que o Aluno visualize, logo após o login, seu nome completo, o nome do instrutor, o plano ativo e a academia associada[cite: 37]. | [cite_start]MÉDIA [cite: 37] |
| RF13 | [cite_start]O sistema deve permitir que o Aluno acesse a tela de Ficha de Treino atual, contendo exercícios numerados, nome do exercício, peso, repetições e séries[cite: 37]. | [cite_start]MÉDIA [cite: 37] |

### 2.2. Requisitos do Instrutor

| Identificador | Descrição | Prioridade |
| :--- | :--- | :--- |
| RF14 | Permitir login de Instrutor com usuário e senha. [cite_start]Exibir mensagem de erro quando não coincidirem[cite: 37]. | [cite_start]ALTA [cite: 37] |
| RF15 | [cite_start]Após login, exibir cabeçalho com Cadastro (nome da pessoa/instrutor) e Academia vinculada[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF16 | [cite_start]Disponibilizar a ação "Ver Alunos" que leva à listagem de alunos do instrutor[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF17 | [cite_start]Exibir lista de alunos (NO MÁXIMO 4) clicáveis para abrir ações do aluno[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF18 | [cite_start]Ao selecionar um aluno, exibir o nome do aluno e do instrutor no topo do fluxo[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF19 | [cite_start]Disponibilizar a ação "Montar treino para aluno" a partir do aluno selecionado[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF20 | [cite_start]Na tela de montar treino, exibir o Treino Atual do aluno (quando existir)[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF21 | [cite_start]Permitir montar/editar treino manualmente com até 8 exercícios numerados (1-8), cada um com Nome do exercício, Peso, Repetições e séries[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF22 | [cite_start]Disponibilizar ação "Montar com IA" que preenche os campos de exercícios/peso/repetições automaticamente para o aluno corrente (instrutor pode revisar/editar)[cite: 43]. | [cite_start]BAIXA [cite: 43] |
| RF23 | [cite_start]Permitir SALVAR o treino montado/alterado do aluno[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF24 | [cite_start]Após salvar, manter o usuário na tela do treino e indicar sucesso (confirmação visual)[cite: 43]. | [cite_start]BAIXA [cite: 43] |
| RF25 | [cite_start]Disponibilizar VOLTAR em todas as telas do fluxo do instrutor (para tela anterior)[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF26 | [cite_start]Disponibilizar SAIR (logout) no cabeçalho/área de navegação do instrutor[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF27 | [cite_start]Na listagem do aluno, disponibilizar atalhos para Ver Fichas (treino do aluno) e Ver Avaliações (histórico do aluno)[cite: 43]. | [cite_start]MÉDIA [cite: 43] |
| RF30 | [cite_start]Na tela de fichas do aluno, permitir ver fichas antigas numeradas (Treino 1, 2, 3, 4...)[cite: 43]. | [cite_start]BAIXA [cite: 43] |
| RF31 | [cite_start]Na tela de avaliações do aluno, permitir ver avaliações antigas com Data, Coef. de força, Gordura corporal e Peso[cite: 43]. | [cite_start]MÉDIA [cite: 43] |

### 2.3. Requisitos do Administrador

| Identificador | Descrição | Prioridade |
| :--- | :--- | :--- |
| RF32 | [cite_start]O sistema deve permitir que o Administrador faça login com usuário e senha válidos[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF33 | [cite_start]O sistema deve exibir mensagem de erro quando o login do Administrador for inválido[cite: 43]. | [cite_start]ALTA [cite: 43] |
| RF34 | [cite_start]O sistema deve permitir que o Administrador faça logout a qualquer momento[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF35 | [cite_start]O sistema deve permitir que o Administrador consulte dados de alunos cadastrados[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF36 | [cite_start]O sistema deve permitir que o Administrador adicione novos alunos[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF37 | [cite_start]O sistema deve permitir que o Administrador altere os dados de alunos existentes[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF38 | [cite_start]O sistema deve permitir que o Administrador exclua alunos da base[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF39 | [cite_start]O sistema deve permitir que o Administrador consulte dados de instrutores cadastrados[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF40 | [cite_start]O sistema deve permitir que o Administrador adicione novos instrutores[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF41 | [cite_start]O sistema deve permitir que o Administrador altere os dados de instrutores existentes[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF42 | [cite_start]O sistema deve permitir que o Administrador exclua instrutores da base[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF43 | [cite_start]O sistema deve permitir que o Administrador consulte planos cadastrados[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF44 | [cite_start]O sistema deve permitir que o Administrador adicione novos planos[cite: 49]. | [cite_start]ALTA [cite: 49] |
| RF45 | [cite_start]O sistema deve permitir que o Administrador altere os planos existentes[cite: 49]. | [cite_start]MEDIA [cite: 49] |
| RF46 | [cite_start]O sistema deve permitir que o Administrador exclua planos da base[cite: 49]. | [cite_start]MÉDIA [cite: 49] |
| RF47 | [cite_start]O sistema deve exibir o nome do Administrador e o nome da Academia associada no cabeçalho[cite: 49]. | [cite_start]BAIXA [cite: 49] |

## 3. Requisitos Não Funcionais

[cite_start]Os requisitos não funcionais definem os critérios de qualidade do sistema[cite: 57].

| Identificador | Descrição | Categoria |
| :--- | :--- | :--- |
| RNF01 | [cite_start]O tempo de resposta para carregar uma Ficha de Treino não deve exceder 2 segundos, mesmo com um grande volume de dados[cite: 58]. | [cite_start]ALTA [cite: 58] |
| RNF02 | [cite_start]O sistema deve suportar no mínimo 200 usuários simultâneos sem degradação perceptível de performance[cite: 58]. | [cite_start]ALTA [cite: 58] |
| RNF03 | [cite_start]O sistema deve exigir login e senha para todos os usuários, com criptografia de ponta a ponta para proteger as credenciais[cite: 58]. | [cite_start]ALTA [cite: 58] |
| RNF04 | [cite_start]A interface do usuário deve ser intuitiva e fácil de usar, permitindo que um novo Instrutor aprenda a criar uma Ficha de Treino em no máximo 15 minutos sem treinamento formal[cite: 58]. | [cite_start]ALTA [cite: 58] |
| RNF05 | [cite_start]As mensagens de erro e de sucesso devem ser claras e descritivas, ajudando o usuário a entender o problema e a resolvê-lo sem a necessidade de suporte[cite: 58]. | [cite_start]MÉDIA [cite: 58] |
| RNF06 | [cite_start]O tempo de atividade do sistema deve ser de, no mínimo, 99,8% por mês[cite: 58]. | [cite_start]ALTA [cite: 58] |
| RNF07 | [cite_start]Todas as ações do Administrador (inserção, edição, exclusão) devem ser registradas em logs de auditoria[cite: 58]. | [cite_start]BAIXA [cite: 58] |
| RNF08 | [cite_start]O sistema deve utilizar banco de dados com backup automático diário para evitar perda de informações de alunos, instrutores e planos[cite: 58]. | [cite_start]MÉDIA [cite: 58] |
| RNF09 | [cite_start]A interface de administração deve permitir gerenciar dados (alunos, instrutores, planos) sem necessidade de conhecimento técnico avançado[cite: 58]. | [cite_start]BAIXA [cite: 58] |

---
[cite_start]*Documento de requisitos elaborado por Rafael Moraes Trevizan [cite: 4] [cite_start]em 22/08/2025[cite: 5].*
