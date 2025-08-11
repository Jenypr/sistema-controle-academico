# sistema-controle-academico

Documentação do projeto desenvolvido como atividade da disciplina de APOO

---

## **Visão do Produto**

---

**Objetivo:**  
Este sistema tem como objetivo gerenciar alunos, professores, cursos e turmas de cursos livres, permitindo controle de frequência, notas e emissão de certificados.

---

**Público-Alvo:**  
Usuários como coordenadores, professores e equipe administrativa de instituições de ensino que oferecem cursos livres.

---

**Principais Funcionalidades**  
- Cadastro e gerenciamento de alunos, professores e cursos.  
- Controle de turmas e matrículas.  
- Registro e consulta de frequência e notas.  
- Emissão de certificados para alunos aprovados.  
- Relatórios de desempenho e participação.

---

**Restrições e Premissas**  
- Desenvolvido para uso via navegador (sistema web).  
- Interface responsiva e amigável.  
- Baseado no estudo de caso de Banco de Dados (cursos livres).  
- Tecnologias previstas: HTML, CSS, JavaScript, Python, SQL.

---

## **Casos de Uso**

Os principais casos de uso identificados são:  
1. Realizar cadastro de aluno.  
2. Registrar frequência e notas.  
3. Emitir certificados de conclusão.

![Diagrama de Casos de Uso](./imagens/diagrama-casos-de-uso.png)

---

### **Descrição dos Casos de Uso**

#### **Caso de Uso 1 – Cadastrar Aluno**
- **Atores:** Coordenador, Administrador  
- **Fluxo Principal:**  
  1. O usuário acessa a área de cadastro de alunos no sistema.  
  2. O usuário insere todas as informações necessárias do aluno, incluindo nome completo, CPF, telefone, e-mail e curso desejado, podendo também adicionar observações ou dados complementares.  
  3. O sistema valida as informações e salva os dados no banco de dados, confirmando o cadastro com uma mensagem de sucesso.  
- **Fluxos Alternativos:**  
  - **A1 – Inclusão de informações adicionais:**  
    1. O usuário opta por inserir dados extras, como endereço, documentos adicionais ou observações internas.  
    2. O sistema armazena essas informações junto aos dados obrigatórios e confirma o cadastro.  
- **Pré-condições:** Usuário autenticado com permissão de cadastro.  
- **Pós-condições:** Aluno cadastrado e disponível para matrícula em turmas.

---

#### **Caso de Uso 2 – Registrar Frequência e Notas**
- **Atores:** Professor  
- **Fluxo Principal:**  
  1. O professor acessa a turma desejada no sistema.  
  2. O professor seleciona o aluno e registra a presença (presente ou ausente) e insere as notas das avaliações realizadas, especificando o tipo de avaliação e data.  
  3. O sistema valida e grava os dados no banco de dados, confirmando a operação.  
- **Fluxos Alternativos:**  
  - **A1 – Registro parcial:**  
    1. O professor registra apenas a frequência ou apenas as notas em um primeiro momento.  
    2. O sistema salva as informações parciais e permite complementação posterior.  
  - **A2 – Alteração antes de salvar:**  
    1. O professor identifica um valor incorreto e o altera antes de concluir o registro.  
    2. O sistema atualiza os dados e confirma a alteração no momento do salvamento final.  
- **Pré-condições:** Turma e alunos cadastrados.  
- **Pós-condições:** Frequência e notas atualizadas no sistema.

---

#### **Caso de Uso 3 – Emitir Certificado**
- **Atores:** Administrador, Coordenador  
- **Fluxo Principal:**  
  1. O usuário acessa a área de emissão de certificados no sistema.  
  2. O usuário seleciona o aluno aprovado e define as opções de emissão, como modelo, personalizações e formato de saída.  
  3. O sistema gera o certificado com os dados do aluno e do curso.  
  4. O sistema disponibiliza o certificado para download ou impressão.  
- **Fluxos Alternativos:**  
  - **A1 – Personalização do certificado:**  
    1. O usuário opta por inserir informações adicionais, como dedicatória, selo especial ou logotipo personalizado.  
    2. O sistema aplica as alterações e emite o certificado personalizado.  
  - **A2 – Escolha do formato de emissão:**  
    1. O usuário seleciona um formato de arquivo diferente (PDF, PNG, DOC).  
    2. O sistema gera o certificado no formato escolhido e disponibiliza para download ou impressão.  
- **Pré-condições:** Aluno aprovado no curso.  
- **Pós-condições:** Certificado emitido e registrado no sistema.

---

## **Modelo Conceitual**

O modelo conceitual representa as classes de análise do sistema, com seus principais atributos e relacionamentos.

![Diagrama de Classes](./imagens/modelo-conceitual.png)

---

### **Descrição das Classes**

- **Aluno**: Representa os estudantes matriculados. Atributos incluem `idAluno`, `nome`, `email`,`telefone`, `dataNascimento`,`cpf`.  
- **Professor**: Representa os docentes. Atributos incluem `idProfessor`, `nome`, `email`, `telefone`, `formacao`.  
- **Curso**: Contém informações sobre cursos livres. Atributos incluem `idCurso`, `idCurso`, `nome`, `descricao`, `cargaHoraria`.  
- **Turma**: Representa uma oferta de curso em um período específico. Atributos incluem `idTurma`, `periodo`, `horario`.  
- **Matricula**: Relaciona alunos a turmas. Atributos incluem `idMatricula`, `dataMatricula`, `status`.  
- **Frequencia**: Registra presença ou falta de alunos. Atributos incluem `idFrequencia`, `dataAula`.  
- **Nota**: Guarda as avaliações dos alunos. Atributos incluem `idNota`, `valor`, `dataLancamento`.  
- **Certificado**: Documento gerado para alunos aprovados. Atributos incluem `idCertificado`,`nome`,`matricula`,`dataEmissao`.

---

## **Tecnologias Utilizadas**
- Documentação escrita em Markdown.  
- Diagramas elaborados com Astah.  
- Repositório hospedado no GitHub.  

---

## **Equipe**
- Jenyffer Danily de Souza Araújo – Matrícula: 20231011110015  
- Anna Alyssia Dantas de Medeiros – Matrícula: 20251011110041  

---

## **Repositório no GitHub**
🔗 [Acesse o projeto no GitHub](https://github.com/Jenypr/sistema-controle-academico)