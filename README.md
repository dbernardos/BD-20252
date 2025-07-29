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
```

---

## 📦 Banco de Dados NoSQL (MongoDB Atlas)
- Coleção: historico_alunos
- Cada documento armazena:
-- aluno_id: ID do aluno (vinculado ao MySQL)
-- atividades: array com projetos, eventos, etc.
-- observacoes: anotações de professores
-- habilidades_extra: array com soft skills

---

## 💻 Aplicação PHP
### Funcionalidades
- Recebe o id do aluno pela URL (ex: painel_aluno.php?id=1)
- Busca os dados principais no MySQL
- Busca o histórico no MongoDB
- Exibe tudo integrado em uma página web

### Como Executar
- Inicie o Apache e MySQL no XAMPP.
- Coloque o arquivo painel_aluno.php na pasta htdocs.
- Acesse no navegador: http://localhost/escola/painel_aluno.php?id=1
