# Casos de Uso

## Caso de Uso 1: Cadastrar Aluno
- **Atores:** Coordenador, Administrador
- **Fluxo Principal:**
  1. O usuário acessa a área de cadastro.
  2. Preenche os dados do aluno (nome, CPF, contato, etc.).
  3. O sistema salva as informações no banco de dados.

- **Fluxos Alternativos:**
  - Dados inválidos impedem o cadastro.
- **Pré-condições:** O usuário deve estar logado com permissão de cadastro.
- **Pós-condições:** Aluno cadastrado e disponível para matrícula em turmas.

## Caso de Uso 2: Registrar Frequência e Notas
- **Atores:** Professor
- **Fluxo Principal:**
  1. O professor acessa a turma desejada.
  2. Seleciona o aluno e insere presença e notas.
  3. O sistema grava os dados.

- **Fluxos Alternativos:**
  - Caso o professor não esteja vinculado à turma, o acesso é negado.
- **Pré-condições:** Turma e alunos devem estar cadastrados.
- **Pós-condições:** Frequência e notas atualizadas.

## Caso de Uso 3: Emitir Certificado
- **Atores:** Administrador, Coordenador
- **Fluxo Principal:**
  1. O sistema verifica se o aluno foi aprovado no curso.
  2. Gera o certificado com os dados do aluno e do curso.
  3. Disponibiliza o certificado para download.
- **Fluxos Alternativos:**
  - Caso o aluno não tenha sido aprovado, o certificado não é emitido.
- **Pré-condições:** Aluno deve estar aprovado.
- **Pós-condições:** Certificado emitido.