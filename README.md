# dr-cbd-platform
Plataforma MVP para gerenciamento de prescrições (C#, .NET)
# 🩺 Dr. CBD — Plataforma MVP de Prescrições

**Descrição curta**  
Plataforma MVP para gerenciamento de prescrições e cadastro de usuários voltada para medicamentos à base de canabidiol. Projeto acadêmico com foco em backend, modelagem de dados e integração entre perfis: Paciente, Médico e Fornecedor.

---

## 📌 Índice
- Sobre
- Tecnologias
- Funcionalidades
- Como executar (local)
- Configuração (variáveis)
- Endpoints principais (resumo)
- Estrutura do projeto
- Diagramas e documentação
- Testes
- Docker (opcional)
- Contribuição
- Licença
- Autor / Contato

---

## 🧾 Sobre
Este repositório contém o backend do MVP desenvolvido durante a graduação em Análise e Desenvolvimento de Sistemas (UniCEUB). O objetivo foi entregar um protótipo funcional que permita cadastro de usuários (Paciente, Médico, Fornecedor), criação e gerenciamento de prescrições, e um controle básico de estoque para fornecedores.

---

## 🛠 Tecnologias
- **Back-end:** C# / .NET 6 (ou superior)  
- **Banco de dados:** SQL Server (ou LocalDB)  
- **Versionamento:** Git / GitHub  
- **Modelagem:** UML (diagramas na pasta `/diagrams`)  
- **Outros:** EF Core (opcional), JWT (autenticação), Swagger (documentação de API)

---

## ✨ Funcionalidades (MVP)
- Cadastro de usuários: Paciente, Médico, Fornecedor  
- Autenticação / Login (JWT)  
- Endpoints CRUD para prescrições  
- Endpoints para visualização e controle de estoque (fornecedores)  
- Modelagem de requisitos e diagramas UML para suporte ao desenvolvimento

---

## ▶️ Como executar (local)
**Pré-requisitos**
- .NET 6 SDK+ instalado: https://dotnet.microsoft.com  
- SQL Server ou LocalDB (ou usar docker-compose para DB)  
- Git

**Passos**
```bash
# 1) clonar
git clone https://github.com/SEU_USUARIO/dr-cbd-platform.git
cd dr-cbd-platform

# 2) restaurar pacotes
dotnet restore

# 3) aplicar migrações (se o projeto usar EF Core)
dotnet ef database update

# 4) executar
dotnet run --project src/DrCbd.Api

`chore: add initial README`
