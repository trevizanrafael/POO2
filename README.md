# README - Sistema de Gestão de Academias GymFlow

Este documento fornece uma visão geral detalhada do sistema GymFlow, um software de gestão para academias. Ele descreve os objetivos do sistema, os diferentes tipos de usuários, e os requisitos funcionais e não funcionais.

## 1. Visão Geral do Sistema

O GymFlow é um sistema de gestão projetado para centralizar e otimizar os processos administrativos e operacionais de uma academia. O objetivo principal é automatizar tarefas rotineiras, como o controle de alunos, a gestão financeira e a criação de treinos, permitindo que a equipe se concentre em oferecer um serviço de maior qualidade aos alunos. A implementação deste sistema visa transformar operações manuais em um fluxo de trabalho digital e eficiente , buscando otimizar o tempo da equipe e melhorar a retenção de alunos através de um acompanhamento personalizado.

O sistema foi projetado para atender às necessidades de três tipos de usuários:

* **Administrador:** Ferramenta para gerenciar cadastros de alunos, instrutores, planos e academias.
* **Instrutor:** Ferramenta de produtividade para cadastrar fichas de treino, acompanhar a evolução dos alunos por meio de avaliações físicas e personalizar os exercícios.
* **Aluno:** Acesso fácil à sua ficha de treino, histórico de pagamentos e acompanhamento de seu progresso através dos resultados das avaliações físicas.

## 2. Requisitos Funcionais

A seguir estão detalhados os requisitos funcionais do sistema, categorizados por perfil de usuário.

### 2.1. Requisitos do Aluno

| Identificador | Descrição | Prioridade |
| :--- | :--- | :--- |
| RF01 | O sistema deve permitir que o Aluno faça login com usuário e senha válidos. | ALTA  |
| RF02 | O sistema deve exibir mensagem de erro quando o login do Aluno for inválido. | ALTA  |
| RF03 | O sistema deve permitir que o Aluno visualize sua Ficha de Treino atual, contendo exercícios, peso, repetições e séries. | ALTA  |
| RF04 | O sistema deve permitir que o Aluno visualize o nome de seu Instrutor responsável. | ALTA  |
| RF05 | O sistema deve permitir que o Aluno visualize seu Plano de Treino e a Academia onde está cadastrado. | MÉDIA  |
| RF06 | O sistema deve permitir que o Aluno visualize o histórico de Fichas de Treino anteriores. | MÉDIA  |
| RF07 | O sistema deve permitir que o Aluno visualize os resultados de Avaliações Físicas (coeficiente de força, gordura corporal, peso e data). | MÉDIA  |
| RF08 | O sistema deve permitir que o Aluno consulte o histórico de Avaliações Físicas antigas. | MÉDIA  |
| RF09 | O sistema deve permitir que o Aluno saia da aplicação (logout). | ALTA  |
| RF10 | O sistema deve permitir que o Aluno navegue entre telas (voltar às opções anteriores). | ALTA  |
| RF11 | O sistema deve numerar e organizar as fichas de treino do Aluno de forma sequencial (ex.: Treino 1, Treino 2...). | BAIXA  |
| RF12 | O sistema deve permitir que o Aluno visualize, logo após o login, seu nome completo, o nome do instrutor, o plano ativo e a academia associada. | MÉDIA  |
| RF13 | O sistema deve permitir que o Aluno acesse a tela de Ficha de Treino atual, contendo exercícios numerados, nome do exercício, peso, repetições e séries. | MÉDIA  |

### 2.2. Requisitos do Instrutor

| Identificador | Descrição | Prioridade |
| :--- | :--- | :--- |
| RF14 | Permitir login de Instrutor com usuário e senha. Exibir mensagem de erro quando não coincidirem. | ALTA  |
| RF15 | Após login, exibir cabeçalho com Cadastro (nome da pessoa/instrutor) e Academia vinculada. | ALTA  |
| RF16 | Disponibilizar a ação "Ver Alunos" que leva à listagem de alunos do instrutor. | ALTA  |
| RF17 | Exibir lista de alunos (NO MÁXIMO 4) clicáveis para abrir ações do aluno. | ALTA  |
| RF18 | Ao selecionar um aluno, exibir o nome do aluno e do instrutor no topo do fluxo. | ALTA  |
| RF19 | Disponibilizar a ação "Montar treino para aluno" a partir do aluno selecionado. | ALTA  |
| RF20 | Na tela de montar treino, exibir o Treino Atual do aluno (quando existir). | ALTA  |
| RF21 | Permitir montar/editar treino manualmente com até 8 exercícios numerados (1-8), cada um com Nome do exercício, Peso, Repetições e séries. | ALTA  |
| RF22 | Disponibilizar ação "Montar com IA" que preenche os campos de exercícios/peso/repetições automaticamente para o aluno corrente (instrutor pode revisar/editar). | BAIXA  |
| RF23 | Permitir SALVAR o treino montado/alterado do aluno. | ALTA  |
| RF24 | Após salvar, manter o usuário na tela do treino e indicar sucesso (confirmação visual). | BAIXA  |
| RF25 | Disponibilizar VOLTAR em todas as telas do fluxo do instrutor (para tela anterior). | ALTA  |
| RF26 | Disponibilizar SAIR (logout) no cabeçalho/área de navegação do instrutor. | ALTA  |
| RF27 | Na listagem do aluno, disponibilizar atalhos para Ver Fichas (treino do aluno) e Ver Avaliações (histórico do aluno). | MÉDIA  |
| RF30 | Na tela de fichas do aluno, permitir ver fichas antigas numeradas (Treino 1, 2, 3, 4...). | BAIXA  |
| RF31 | Na tela de avaliações do aluno, permitir ver avaliações antigas com Data, Coef. de força, Gordura corporal e Peso. | MÉDIA  |

### 2.3. Requisitos do Administrador

| Identificador | Descrição | Prioridade |
| :--- | :--- | :--- |
| RF32 | O sistema deve permitir que o Administrador faça login com usuário e senha válidos. | ALTA  |
| RF33 | O sistema deve exibir mensagem de erro quando o login do Administrador for inválido. | ALTA  |
| RF34 | O sistema deve permitir que o Administrador faça logout a qualquer momento. | ALTA  |
| RF35 | O sistema deve permitir que o Administrador consulte dados de alunos cadastrados. | ALTA  |
| RF36 | O sistema deve permitir que o Administrador adicione novos alunos. | ALTA  |
| RF37 | O sistema deve permitir que o Administrador altere os dados de alunos existentes. | ALTA  |
| RF38 | O sistema deve permitir que o Administrador exclua alunos da base. | ALTA  |
| RF39 | O sistema deve permitir que o Administrador consulte dados de instrutores cadastrados. | ALTA  |
| RF40 | O sistema deve permitir que o Administrador adicione novos instrutores. | ALTA  |
| RF41 | O sistema deve permitir que o Administrador altere os dados de instrutores existentes. | ALTA  |
| RF42 | O sistema deve permitir que o Administrador exclua instrutores da base. | ALTA  |
| RF43 | O sistema deve permitir que o Administrador consulte planos cadastrados. | ALTA  |
| RF44 | O sistema deve permitir que o Administrador adicione novos planos. | ALTA  |
| RF45 | O sistema deve permitir que o Administrador altere os planos existentes. | MEDIA  |
| RF46 | O sistema deve permitir que o Administrador exclua planos da base. | MÉDIA  |
| RF47 | O sistema deve exibir o nome do Administrador e o nome da Academia associada no cabeçalho. | BAIXA  |

## 3. Requisitos Não Funcionais

Os requisitos não funcionais definem os critérios de qualidade do sistema.

| Identificador | Descrição | Categoria |
| :--- | :--- | :--- |
| RNF01 | O tempo de resposta para carregar uma Ficha de Treino não deve exceder 2 segundos, mesmo com um grande volume de dados. | ALTA  |
| RNF02 | O sistema deve suportar no mínimo 200 usuários simultâneos sem degradação perceptível de performance. | ALTA  |
| RNF03 | O sistema deve exigir login e senha para todos os usuários, com criptografia de ponta a ponta para proteger as credenciais. | ALTA  |
| RNF04 | A interface do usuário deve ser intuitiva e fácil de usar, permitindo que um novo Instrutor aprenda a criar uma Ficha de Treino em no máximo 15 minutos sem treinamento formal. | ALTA  |
| RNF05 | As mensagens de erro e de sucesso devem ser claras e descritivas, ajudando o usuário a entender o problema e a resolvê-lo sem a necessidade de suporte. | MÉDIA  |
| RNF06 | O tempo de atividade do sistema deve ser de, no mínimo, 99,8% por mês. | ALTA  |
| RNF07 | Todas as ações do Administrador (inserção, edição, exclusão) devem ser registradas em logs de auditoria. | BAIXA  |
| RNF08 | O sistema deve utilizar banco de dados com backup automático diário para evitar perda de informações de alunos, instrutores e planos. | MÉDIA  |
| RNF09 | A interface de administração deve permitir gerenciar dados (alunos, instrutores, planos) sem necessidade de conhecimento técnico avançado. | BAIXA  |

---
*Documento de requisitos elaborado por Rafael Moraes Trevizan em 22/08/2025.*
