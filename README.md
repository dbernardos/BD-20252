# 🎓 Projeto 1: Sistema da Escola Técnica

**Disciplina:** Banco de Dados  
**Curso:** Técnico em Desenvolvimento de Sistemas  
**Aluno(a):** [Seu Nome]  
**Turma:** [Sua Turma]  
**Data de Entrega:** [dd/mm/aaaa]  

---

## 🎯 Objetivo
Integrar um banco de dados relacional (**MySQL**) com um banco NoSQL (**MongoDB**) em uma aplicação simples usando **PHP**, exibindo dados de alunos e seu histórico de atividades em uma página web.

---

## 🛠️ Tecnologias Utilizadas
- 💾 MySQL (banco relacional)
- 📦 MongoDB Atlas (banco NoSQL na nuvem)
- 💬 PHP (integração e exibição)
- 🔗 GitHub (versionamento)
- 🖥️ XAMPP (servidor local)

---

## 🗄️ Banco de Dados Relacional (MySQL)

### Estrutura das Tabelas
```sql
-- Tabela: alunos
id (INT, PK), nome (VARCHAR), email (VARCHAR), data_nascimento (DATE)

-- Tabela: cursos
id (INT, PK), nome_curso (VARCHAR), carga_horaria (INT)

-- Tabela: matriculas
id (INT, PK), aluno_id (INT, FK), curso_id (INT, FK), data_matricula (DATE)
