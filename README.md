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
* **Front-End:** HTML5 e CSS3 para estrutura, layout e responsividade
* **Back-End:** Java para a lógica de negócio e integração
* **Banco de Dados:** MySQL para modelagem e armazenamento dos dados de salas, professores e horários

**Recursos Implementados:**
* Consulta de disponibilidade de salas em tempo real
* Mapeamento dos horários docentes por turno e bloco
* Painel com indicação visual de salas disponíveis e ocupadas
* Interface simples e intuitiva adaptada para o uso da equipe de limpeza

---

## 📦 Estrutura do Projeto

```text
clear_spaces/
├── src/
│   ├── main/
│   │   ├── java/       # Classes e controllers em Java
│   │   └── webapp/     # Estrutura web (HTML, CSS, recursos)
│   │       ├── css/    # Estilização e design
│   │       └── index.html
├── database/           # Scripts de criação e população do MySQL
├── documentacao/       # Links das Sprints, relatórios e diagramas
└── README.md           # Documentação do projeto
