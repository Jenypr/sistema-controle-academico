# Casos de Uso

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

## **Caso de Uso 2 – Registrar Frequência**
- **Atores:** Professor  
- **Fluxo Principal:**  
  1. O professor acessa a turma no sistema.  
  2. Seleciona o aluno e registra a presença (presente ou ausente).  
  3. O sistema valida e grava a informação no banco de dados, confirmando o registro.  
- **Fluxos Alternativos:**  
  - **A1 – Registro parcial:**  
    1. O professor registra a frequência parcialmente, podendo completar depois.  
    2. O sistema salva o registro parcial e permite complementação posterior.  
  - **A2 – Alteração antes de salvar:**  
    1. O professor corrige algum valor antes de finalizar o registro.  
    2. O sistema atualiza o dado e confirma a alteração ao salvar.  
- **Pré-condições:** Turma e alunos cadastrados.  
- **Pós-condições:** Frequência atualizada no sistema.

---

## **Caso de Uso 3 – Registrar Notas**
- **Atores:** Professor  
- **Fluxo Principal:**  
  1. O professor acessa a turma no sistema.  
  2. Seleciona o aluno e insere as notas das avaliações, informando tipo e data.  
  3. O sistema valida e grava as notas no banco de dados, confirmando o registro.  
- **Fluxos Alternativos:**  
  - **A1 – Registro parcial:**  
    1. O professor registra notas parcialmente, podendo completar depois.  
    2. O sistema salva o registro parcial e permite complementação posterior.  
  - **A2 – Alteração antes de salvar:**  
    1. O professor corrige algum valor antes de finalizar o registro.  
    2. O sistema atualiza o dado e confirma a alteração ao salvar.  
- **Pré-condições:** Turma e alunos cadastrados.  
- **Pós-condições:** Notas atualizadas no sistema.


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