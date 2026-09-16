# Clear Spaces — Gestão de Limpeza SENAI

Projeto Integrador desenvolvido no curso **Técnico em Desenvolvimento de Sistemas** do SENAI, sob orientação do professor **Wesley**. O **Clear Spaces** é uma solução web desenvolvida para otimizar e organizar a rotina do setor de limpeza através da integração de dados de ocupação de salas e horários dos docentes.

---

## 📚 Contexto e Problema

Nas instituições de ensino, a higienização das salas precisa acompanhar a dinâmica contínua de aulas e trocas de professores. O **Clear Spaces** conecta a agenda de horários docentes aos serviços de limpeza do SENAI, permitindo que a equipe de conservação identifique em tempo real as salas disponíveis e execute o serviço de forma mais eficiente, previsível e organizada.

---

## 🎯 Objetivos do Projeto

Desenvolver uma aplicação web interativa que:
* **Vincule a agenda docente às salas:** Mapeie os horários de aula dos professores para identificar automaticamente os horários vagos nas salas.
* **Otimize a rotina da limpeza:** Indique em tempo real os locais disponíveis para o trabalho das faxineiras.
* **Aumente a eficiência operacional:** Evite interrupções desnecessárias em salas ocupadas e melhore a organização da equipe.
* **Ofereça controle visual:** Facilite o acompanhamento das tarefas e do status de conservação de cada ambiente do SENAI.

---

## 👥 Equipe — PRISM DEVELOPMENT

| Integrante | Funções / Responsabilidades |
| :--- | :--- |
| **Letícia Salvador Ciscare** | Líder • Front-End • Design |
| **Julio Cesar Pires Miranda dos Santos** | Full-Stack |
| **Vinícius Bernardi Sant'Ana** | Front-End • Design • Analista • Banco de Dados |
| **Luan Fernandes Da Silva** | Banco de Dados |

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

```text
clearSpaces/
├── FRONTEND/
│   ├── HTML/
│   │   ├── index.html
│   │   ├── cadastros.html
│   │   ├── gerente.html
│   │   ├── operacional.html
│   │   ├── professor.html
│   │   └── ... (formulários, listas e checklists)
│   ├── JS/
│   │   ├── common.js
│   │   ├── login.js
│   │   └── ... (scripts de controle da interface)
│   └── style.css
│
├── BACKEND (br.com.api.clearSpaces)/
│   ├── controller/      # Endpoints da API REST
│   ├── dto/             # Objetos de transferência de dados
│   ├── entity/          # Mapeamento das tabelas do banco
│   ├── repository/      # Interfaces de acesso ao MySQL
│   └── service/         # Regras de negócio da aplicação
│
└── DATABASE/
    └── scripts.sql      # Scripts de criação e população no MySQL Workbench
