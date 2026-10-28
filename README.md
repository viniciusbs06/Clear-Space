# Clear Spaces — Gestão de Limpeza SENAI

Projeto Integrador desenvolvido no curso **Técnico em Desenvolvimento de Sistemas** do SENAI, sob orientação do professor **Wesley**. O **Clear Spaces** é uma solução web desenvolvida para otimizar e organizar a rotina do setor de limpeza através da integração de dados de ocupação de salas e horários dos docentes.

---

## 📚 Contexto e Problema

Nas instituições de ensino, a higienização das salas precisa acompanhar a dinâmica contínua de aulas e trocas de professores. O **Clear Spaces** conecta a agenda de horários docentes aos serviços de limpeza do SENAI, permitindo que a equipe de conservação identifique em tempo real as salas disponíveis e execute o serviço de forma mais eficiente, previsível e organizada.

---

## 🎯 Objetivos do Projeto

Desenvolver uma aplicação web interativa que:
- **Vincule a agenda docente às salas:** Mapeie os horários de aula dos professores para identificar automaticamente os horários vagos nas salas.
- **Otimize a rotina da limpeza:** Indique em tempo real os locais disponíveis para o trabalho da equipe de limpeza.
- **Aumente a eficiência operacional:** Evite interrupções desnecessárias em salas ocupadas e melhore a organização da equipe.
- **Ofereça controle visual:** Facilite o acompanhamento das tarefas e do status de conservação de cada ambiente do SENAI.

---

## 👥 Equipe — PRISM DEVELOPMENT

| Integrante | Funções / Responsabilidades |
| :--- | :--- |
| **Letícia Salvador Ciscare** | Líder • Front-End • Design |
| **Julio Cesar Pires Miranda dos Santos** | Full-Stack |
| **Vinícius Bernardi Sant'Ana** | Analista • Front-End • Banco de Dados |
| **Luan Fernandes Da Silva** | Banco de Dados • Design |

---

## 🛠️ Implementação Técnica

**Tecnologias Utilizadas:**
- **Front-End:** HTML5, CSS3 (`style.css`) e JavaScript para a interface web interativa
- **Back-End:** Java (Spring Boot / API Restful) com arquitetura MVC/DTO
- **Banco de Dados:** MySQL (`clearSpaces`) para persistência de dados via JPA/Hibernate

**Recursos Implementados:**
- Gestão completa de ambientes, cadastros e cronogramas de limpeza
- Controle de atribuições, tarefas e checklist operacional dos funcionários
- Registro e acompanhamento do histórico de ocorrências pelo gerente
- Autenticação e gestão de acessos para perfis de gerência, operação e docentes
- Consulta e mapeamento de disponibilidade de salas por turno/período

---

## 📦 Estrutura do Projeto

- **FRONTEND/**
  * **HTML/** (`index.html`, `cadastros.html`, `gerente.html`, `operacional.html`, `professor.html`, etc.)
  * **JS/** (`common.js`, `login.js`, etc.)
  * `style.css`
- **BACKEND (`br.com.api.clearSpaces`)/**
  * **controller/** (Endpoints da API REST)
  * **dto/** (Objetos de transferência de dados)
  * **entity/** (Mapeamento das tabelas do banco)
  * **repository/** (Interfaces de acesso ao MySQL)
  * **service/** (Regras de negócio da aplicação)
- **DATABASE/**
  * `scripts.sql` (Scripts de criação e população no MySQL Workbench)

---

## 🔗 Links e Documentações

  * [Planilha de Planejamento (Google Sheets)](https://docs.google.com/spreadsheets/d/1A0A2PTlN-N85IHBUX_GJvX5Yg3KyZ7VHLuMK3ojl1WM/edit?gid=0#gid=0)
  * [Documento de Acompanhamento (Google Docs)](https://docs.google.com/document/d/1AYgvl47JNWB99ZoGaq5CfaBvfCuL6UGqTqc5rXoqGfo/edit?tab=t.0)

---

## 🚀 Como Utilizar

### 1. Extração dos Arquivos
Localize o arquivo compactado e extraia a pasta.

<img width="750" alt="Localizando pasta compactada" src="https://github.com/user-attachments/assets/5f7d0c8c-6c40-43a1-b725-c73946eee49d" />

<img width="750" alt="Extraindo arquivos" src="https://github.com/user-attachments/assets/4add24b6-b331-4155-ac47-486fe92c94a0" />

---

### 2. Abrindo o Back-End no IntelliJ IDEA
1. Abra o IntelliJ IDEA e clique no botão **Open** para abrir o projeto.

<img width="750" alt="Abrindo o IntelliJ IDEA" src="https://github.com/user-attachments/assets/1e9df305-293d-4a37-9fa0-88ca83d60774" />

2. Selecione a pasta **BACKEND** (localizada dentro da pasta principal extraída).

<img width="750" alt="Selecionando a pasta BACKEND" src="https://github.com/user-attachments/assets/f9ee67e4-ca48-4d43-af48-e0cab8f0b4ff" />

---

### 3. Configuração Inicial do Banco de Dados
Edite o arquivo `application.properties` alterando a linha para `spring.sql.init.mode=always`. Isso fará com que o Spring inicialize e popule o banco de dados na primeira execução.

<img width="750" alt="Configurando application.properties para always" src="https://github.com/user-attachments/assets/3282f037-9616-4213-bfe2-6958b5802c48" />

<img width="750" alt="Alterando propriedade para always" src="https://github.com/user-attachments/assets/8ea7ece1-73c8-493b-9d61-abc4fa597d7d" />

---

### 4. Executando o Back-End
Abra o arquivo `ClearSpacesApplication.java` e execute a aplicação (botão Play verde).

<img width="750" alt="Executando a aplicação Spring Boot" src="https://github.com/user-attachments/assets/1d4fdd23-6b7c-4e9f-a795-e64520174e3f" />

---

### 5. Ajuste Pós-Inicialização do Banco
Após o sistema iniciar com sucesso, altere novamente a propriedade no `application.properties` para `spring.sql.init.mode=never`. 

> ⚠️ **Importante:** Se mantiver como `always`, a cada nova inicialização o Spring tentará inserir registros duplicados no banco de dados.

<img width="750" alt="Alterando propriedade para never" src="https://github.com/user-attachments/assets/ac974750-0c6d-4e65-a1e8-f4be752e6b7d" />

---

### 6. Abrindo o Front-End no VS Code
1. Abra o **Visual Studio Code** e clique em **Open Folder...** (Abrir Pasta).

<img width="750" alt="Abrindo pasta no VS Code" src="https://github.com/user-attachments/assets/10c898e0-8aad-4ec1-afeb-d16a9ffbb90f" />

2. Selecione a pasta **FRONTEND** dentro da pasta principal.

<img width="750" alt="Selecionando pasta FRONTEND" src="https://github.com/user-attachments/assets/d0f00543-2ae6-4c0b-a49f-4de064fe5a56" />

---

### 7. Verificando o Live Server
Acesse a aba de extensões do seu VS Code e verifique se a extensão **Live Server** está instalada e habilitada. Caso não esteja, instale-a.

<img width="750" alt="Verificando a extensão Live Server" src="https://github.com/user-attachments/assets/1306c7da-d12f-46ea-a592-345014410172" />

---

### 8. Executando a Aplicação Web
Volte para o navegador de arquivos do VS Code, abra o arquivo `index.html` e clique no botão **Go Live!** no canto inferior direito para rodar a aplicação localmente.

<img width="750" alt="Iniciando com Go Live no VS Code" src="https://github.com/user-attachments/assets/97807c8d-49b1-4e91-bfe7-2dcfe0f3d84e" />

## 👥 Perfis Cadastrados Automaticamente

### Funcionários
| Função | Matrícula | Nome | Período ID | CPF | Senha |
| :--- | :--- | :--- | :---: | :--- | :--- |
| Gerente | `FUNC-1234` | João Silva | 1 | `11111111111` | `senha123` |
| ASG | `FUNC-1235` | Nicolas Pereira | 2 | `11111111112` | `senha123` |
| Banheirista | `FUNC-1236` | Maria Oliveira | 1 | `11111111114` | `senha123` |
| ASG | `FUNC-1237` | Carlos Souza | 2 | `11111111115` | `senha123` |
| Banheirista | `FUNC-1238` | Ana Santos | 3 | `11111111116` | `senha123` |

### Professores
| Matrícula | Nome | Período ID | CPF | Senha |
| :--- | :--- | :---: | :--- | :--- |
| `PROF-1232` | Vinicius Lira | 3 | `11111111113` | `senha123` |
| `PROF-1233` | Mariana Costa | 1 | `11111111117` | `senha123` |
| `PROF-1234` | Roberto Alves | 2 | `11111111118` | `senha123` |
---

## 🌐 Links da Aplicação 

- **Site:** [https://frontclearspaces.vercel.app](https://frontclearspaces.vercel.app)
- **Landing Page:** [https://landingpageclearspaces.vercel.app](https://landingpageclearspaces.vercel.app)
- **Repositório Back-End:** [https://github.com/julio-cpm/backClearSpaces](https://github.com/julio-cpm/backClearSpaces)
- **Repositório Front-End:** [https://github.com/julio-cpm/frontClearSpaces](https://github.com/julio-cpm/frontClearSpaces)

---

## 📝 Considerações Finais

O **Clear Spaces** resolve um desafio operacional real do SENAI, unindo conceitos de desenvolvimento web, APIs REST em Java e modelagem de banco de dados para entregar valor prático à gestão predial da instituição. Desenvolvido no âmbito do curso Técnico em Desenvolvimento de Sistemas, demonstra a aplicação prática de arquitetura em camadas e design de interfaces focados na rotina de trabalho real.
