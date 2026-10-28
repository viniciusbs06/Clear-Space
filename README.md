# Clear Spaces — Gestão de Limpeza SENAI
 
Projeto Integrador desenvolvido no curso **Técnico em Desenvolvimento de Sistemas** do SENAI, sob orientação do professor **Wesley**. O **Clear Spaces** é uma solução web desenvolvida para otimizar e organizar a rotina do setor de limpeza através da integração de dados de ocupação de salas e horários dos docentes.

---

## 📚 Contexto e Problema

Nas instituições de ensino, a higienização das salas precisa acompanhar a dinâmica contínua de aulas e trocas de professores. O **Clear Spaces** conecta a agenda de horários docentes aos serviços de limpeza do SENAI, permitindo que a equipe de conservação identifique em tempo real as salas disponíveis e execute o serviço de forma mais eficiente, previsível e organizada.

---

## 🎯 Objetivos do Projeto

Desenvolver uma aplicação web interativa que:
* **Vincule a agenda docente às salas:** Mapeie os horários de aula dos professores para identificar automaticamente os horários vagos nas salas.
* **Otimize a rotina da limpeza:** Indique em tempo real os locais disponíveis para o trabalho da equipe de limpeza.
* **Aumente a eficiência operacional:** Evite interrupções desnecessárias em salas ocupadas e melhore a organização da equipe.
* **Ofereça controle visual:** Facilite o acompanhamento das tarefas e do status de conservação de cada ambiente do SENAI.

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
* **Front-End:** HTML5, CSS3 (`style.css`) e JavaScript para a interface web interativa
* **Back-End:** Java (Spring Boot / API Restful) com arquitetura MVC/DTO
* **Banco de Dados:** MySQL (`clearSpaces`) para persistência de dados via JPA/Hibernate

**Recursos Implementados:**
* Gestão completa de ambientes, cadastros e cronogramas de limpeza
* Controle de atribuições, tarefas e checklist operacional dos funcionários
* Registro e acompanhamento do histórico de ocorrências pelo gerente
* Autenticação e gestão de acessos para perfis de gerência, operação e docentes
* Consulta e mapeamento de disponibilidade de salas por turno/período

---

## 📦 Estrutura do Projeto

* **FRONTEND/**
  * **HTML/** (`index.html`, `cadastros.html`, `gerente.html`, `operacional.html`, `professor.html`, etc.)
  * **JS/** (`common.js`, `login.js`, etc.)
  * `style.css`
* **BACKEND (`br.com.api.clearSpaces`)/**
  * **controller/** (Endpoints da API REST)
  * **dto/** (Objetos de transferência de dados)
  * **entity/** (Mapeamento das tabelas do banco)
  * **repository/** (Interfaces de acesso ao MySQL)
  * **service/** (Regras de negócio da aplicação)
* **DATABASE/**
  * `scripts.sql` (Scripts de criação e população no MySQL Workbench)

---

## 🔗 Links e Documentações

* **Sprint 1 (Parcial):**
  * [[Planilha de Planejamento (Google Sheets)](https://docs.google.com/spreadsheets/d/12V4GN4cUz8yyqX4Xnle9iTjXCsKeq625dAWcHrxlSa8/edit?usp=sharing)](https://docs.google.com/spreadsheets/d/1A0A2PTlN-N85IHBUX_GJvX5Yg3KyZ7VHLuMK3ojl1WM/edit?gid=0#gid=0)
  * [Documento de Acompanhamento (Google Docs)](https://docs.google.com/document/d/1AYgvl47JNWB99ZoGaq5CfaBvfCuL6UGqTqc5rXoqGfo/edit?tab=t.0)

---

## 🚀 Como Utilizar

<img width="1021" height="534" alt="Captura de tela 2026-10-28 084845" src="https://github.com/user-attachments/assets/5f7d0c8c-6c40-43a1-b725-c73946eee49d" />
<img width="1117" height="805" alt="Captura de tela 2026-10-28 084853" src="https://github.com/user-attachments/assets/4add24b6-b331-4155-ac47-486fe92c94a0" />
Extraia a pasta compactada
<img width="1919" height="1079" alt="Captura de tela 2026-10-28 085316" src="https://github.com/user-attachments/assets/1e9df305-293d-4a37-9fa0-88ca83d60774" />
Abra o intelliJ e clique no botão para abrir o projeto
<img width="1919" height="1079" alt="Captura de tela 2026-10-28 085348" src="https://github.com/user-attachments/assets/f9ee67e4-ca48-4d43-af48-e0cab8f0b4ff" />
Abra a pasta BACKEND (localizada dentro da pasta principal)
<img width="1919" height="1079" alt="Captura de tela 2026-10-28 085437" src="https://github.com/user-attachments/assets/3282f037-9616-4213-bfe2-6958b5802c48" />
<img width="1919" height="1079" alt="Captura de tela 2026-10-28 090203" src="https://github.com/user-attachments/assets/8ea7ece1-73c8-493b-9d61-abc4fa597d7d" />
Faça uma edição no arquivo aplication.properties para o sistema popular o banco de dados
<img width="1919" height="1079" alt="Captura de tela 2026-10-28 090239" src="https://github.com/user-attachments/assets/1d4fdd23-6b7c-4e9f-a795-e64520174e3f" />
Abra o arquivo ClearSpacesApplication e execute o projeto
<img width="1919" height="1076" alt="Captura de tela 2026-10-28 090303" src="https://github.com/user-attachments/assets/ac974750-0c6d-4e65-a1e8-f4be752e6b7d" />
Altere novamente o arquivo aplication.properties para não popular novamente o banco de dados, caso mantenha o always, toda vez que iniciar o projeto, o spring vai inserir dados repetidos no banco de dados.
<img width="1918" height="1079" alt="Captura de tela 2026-10-28 090332" src="https://github.com/user-attachments/assets/10c898e0-8aad-4ec1-afeb-d16a9ffbb90f" />
Abra o VS Code e clique no botão de abrir pasta
<img width="1919" height="1079" alt="Captura de tela 2026-10-28 090426" src="https://github.com/user-attachments/assets/d0f00543-2ae6-4c0b-a49f-4de064fe5a56" />
Selecione o FRONTEND dentro da pasta principal
<img width="1919" height="1079" alt="Captura de tela 2026-10-28 090520" src="https://github.com/user-attachments/assets/1306c7da-d12f-46ea-a592-345014410172" />
Vá para as dependências do seu VS code e verifique se o Live Server está instalado e habilitado, caso não esteja, instale e o habilite.
<img width="1919" height="1079" alt="Captura de tela 2026-10-28 090545" src="https://github.com/user-attachments/assets/97807c8d-49b1-4e91-bfe7-2dcfe0f3d84e" />
Volte para os arquivos da pasta e abra o index.html e clique no botão Go Live! para rodar a nossa aplicação localmente.

---

## LINKS DA APLICAÇÃO 

 **SITE** <br>
 *https://frontclearspaces.vercel.app*


 **LANDING PAGE** <br>
 *https://landingpageclearspaces.vercel.app*

 **REPOSITORIO COM O BACKEND** <br>
 *https://github.com/julio-cpm/backClearSpaces*

 **REPOSITORIO COM O FRONTEND** <br>
 *https://github.com/julio-cpm/frontClearSpaces*

---

## 📝 Considerações Finais

O **Clear Spaces** resolve um desafio operacional real do SENAI, unindo conceitos de desenvolvimento web, APIs REST em Java e modelagem de banco de dados para entregar valor prático à gestão predial da instituição. Desenvolvido no âmbito do curso Técnico em Desenvolvimento de Sistemas, demonstra a aplicação prática de arquitetura em camadas e design de interfaces focados na rotina de trabalho real.
