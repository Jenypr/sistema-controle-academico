## Modelo Conceitual – Classes de Análise

## Diagrama de Classes
![Diagrama de Classes](./imagens/modelo-conceitual.png)

## Descrição das Classes
 Classe Aluno
- **Atributos:**
  - id_aluno
  - nome
  - cpf
  - email
  - telefone
  - data_nascimento

 Classe Professor
- **Atributos:**
  - id_professor
  - nome
  - email
  - telefone
  - formação

 Classe Curso
- **Atributos:**
  - id_curso
  - nome
  - descrição
  - carga_horaria

 Classe Turma
- **Atributos:**
  - id_turma
  - periodo
  - turno

 Classe Matricula
- **Atributos:**
  - id_matricula
  - data_matricula
  - status

 Classe Certificado
- **Atributos:**
  - id_certificado
  - matricula
  - data_emissao