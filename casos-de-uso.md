# Casos de Uso

## **Caso de Uso 1 – Cadastrar Aluno**
- **Atores:** Coordenador, Administrador  
- **Fluxo Principal:**  
  1. O usuário acessa a área de cadastro.  
  2. Preenche os dados do aluno (nome, CPF, contato, etc.).  
  3. O sistema valida e salva as informações no banco de dados.  
- **Fluxos Alternativos:**  
  - Dados inválidos → o sistema informa o erro e impede o cadastro.  
- **Pré-condições:** Usuário autenticado com permissão de cadastro.  
- **Pós-condições:** Aluno cadastrado e disponível para matrícula em turmas.

---

## **Caso de Uso 2 – Registrar Frequência e Notas**
- **Atores:** Professor  
- **Fluxo Principal:**  
  1. O professor acessa a turma desejada.  
  2. Seleciona o aluno e insere presença e notas.  
  3. O sistema grava os dados no banco de dados.  
- **Fluxos Alternativos:**  
  - Caso o professor não esteja vinculado à turma, o acesso é negado.  
- **Pré-condições:** Turma e alunos cadastrados.  
- **Pós-condições:** Frequência e notas atualizadas no sistema.

---

## **Caso de Uso 3 – Emitir Certificado**
- **Atores:** Administrador, Coordenador  
- **Fluxo Principal:**  
  1. O sistema verifica se o aluno foi aprovado no curso.  
  2. Gera o certificado com os dados do aluno e do curso.  
  3. Disponibiliza o certificado para download ou impressão.  
- **Fluxos Alternativos:**  
  - Caso o aluno não tenha sido aprovado, o certificado não é emitido.  
- **Pré-condições:** Aluno aprovado no curso.  
- **Pós-condições:** Certificado emitido e registrado no sistema.
