# Casos de Uso

## **Caso de Uso 1 – Cadastrar Aluno**
- **Atores:** Coordenador, Administrador  
- **Fluxo Principal:**  
  1. O usuário acessa a área de cadastro.  
  2. Preenche os dados do aluno (nome, CPF, contato, etc.).  
  3. O sistema valida e salva as informações no banco de dados.  
- **Fluxos Alternativos:**  
  - **A1 – Inclusão de informações adicionais:**  
    1. O usuário opta por inserir dados complementares (endereço, documentos extras, observações).  
    2. O sistema salva as informações adicionais junto aos dados obrigatórios e confirma o cadastro.  
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
  - **A1 – Registro parcial:**  
    1. O professor registra apenas a frequência ou apenas as notas em um primeiro momento.  
    2. O sistema salva as informações parciais e permite complementação posterior.  
  - **A2 – Alteração antes de salvar:**  
    1. O professor identifica um valor incorreto e altera antes de concluir o registro.  
    2. O sistema atualiza os dados e confirma a alteração no salvamento final.  
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
  - **A1 – Personalização do certificado:**  
    1. O usuário opta por inserir informações adicionais (dedicatória, selo especial, logotipo extra).  
    2. O sistema aplica as alterações e emite o certificado personalizado.  
  - **A2 – Escolha do formato de emissão:**  
    1. O usuário seleciona um formato de arquivo diferente (PDF, PNG, DOC).  
    2. O sistema gera o certificado no formato escolhido e disponibiliza para download ou impressão.  
- **Pré-condições:** Aluno aprovado no curso.  
- **Pós-condições:** Certificado emitido e registrado no sistema.