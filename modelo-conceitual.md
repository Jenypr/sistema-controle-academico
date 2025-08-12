## **Modelo Conceitual – Classes de Análise**

### **Diagrama de Classes**
![Diagrama de Classes](./imagens/modelo-conceitual.png)

---

### **Descrição das Classes**

#### **Classe: Aluno**
- **Atributos:**
  - `id_aluno` – Identificador único do aluno.
  - `nome` – Nome completo.
  - `cpf` – Cadastro de Pessoa Física.
  - `email` – Endereço de e-mail.
  - `telefone` – Contato telefônico.
  - `data_nascimento` – Data de nascimento do aluno.

---

#### **Classe: Professor**
- **Atributos:**
  - `id_professor` – Identificador único do professor.
  - `nome` – Nome completo.
  - `email` – Endereço de e-mail.
  - `telefone` – Contato telefônico.
  - `formacao` – Formação acadêmica ou área de especialização.

---

#### **Classe: Curso**
- **Atributos:**
  - `id_curso` – Identificador único do curso.
  - `nome` – Nome do curso.
  - `descricao` – Breve descrição do curso.
  - `carga_horaria` – Carga horária total do curso.

---

#### **Classe: Turma**
- **Atributos:**
  - `id_turma` – Identificador único da turma.
  - `periodo` – Período letivo.
  - `turno` – Turno de funcionamento (manhã, tarde, noite).

---

#### **Classe: Matricula**
- **Atributos:**
  - `id_matricula` – Identificador único da matrícula.
  - `data_matricula` – Data em que a matrícula foi realizada.
  - `status` – Situação da matrícula (ativa, concluída, cancelada).

---

#### **Classe: Certificado**
- **Atributos:**
  - `id_certificado` – Identificador único do certificado.
  - `matricula` – Referência à matrícula do aluno.
  - `data_emissao` – Data de emissão do certificado.