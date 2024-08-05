# Documentação da Página: Tela de Perfil do Usuário

## 1. Objetivo
A Tela de Perfil do Usuário permite aos usuários visualizar e editar suas informações pessoais e configurações da conta. Inclui opções para atualizar dados pessoais, alterar a senha e visualizar o histórico de atividades.

## 2. Requisitos
### Funcionalidades
- **Visualização de Perfil**: Exibe informações pessoais do usuário, como nome, email e tipo de usuário.
- **Edição de Perfil**: Permite ao usuário atualizar suas informações pessoais, como nome e email.
- **Alterar Senha**: Opção para alterar a senha da conta do usuário.
- **Histórico de Atividades**: Exibe um histórico das atividades recentes do usuário, como empréstimos e devoluções de livros.
- **Botão de Salvar**: Envia as alterações para o backend e atualiza as informações do perfil.
- **Validação de Dados**: Valida as entradas dos formulários para garantir a correção das informações inseridas.

### Dados Necessários
- **Perfil do Usuário**: Nome, email, tipo de usuário.
- **Histórico de Atividades**: Dados sobre empréstimos e devoluções recentes.

### Requisitos Técnicos
- Integração com o backend para recuperar e atualizar as informações do perfil do usuário.
- Implementação de validação de dados para garantir a integridade das informações inseridas.

## 3. Layout e Design
### Estrutura da Tela
- **Cabeçalho**: Logo do aplicativo e título "Perfil do Usuário".
- **Corpo**:
  - **Visualização de Perfil**: Exibição das informações pessoais do usuário.
  - **Edição de Perfil**:
    - Campo para Nome
    - Campo para Email
    - Botão de Salvar
  - **Alterar Senha**:
    - Campo para Senha Atual
    - Campo para Nova Senha
    - Campo para Confirmar Nova Senha
    - Botão de Alterar Senha
  - **Histórico de Atividades**: Exibição das atividades recentes do usuário.
- **Rodapé**: Links para políticas de privacidade e termos de serviço (opcional).

### Wireframe
- Inclua um wireframe ou mockup da Tela de Perfil do Usuário (se disponível).

### Estilo e Temas
- **Cores**: Utilizar a paleta de cores padrão do aplicativo.
- **Fontes**: Fonte padrão do aplicativo para todos os textos.
- **Botões e Campos de Entrada**: Estilo consistente com o restante do aplicativo, com foco na clareza e usabilidade dos formulários.

## 4. Navegação
### Links e Botões
- **Botão de Salvar**: Envia as alterações do perfil para o backend e atualiza as informações.
- **Botão de Alterar Senha**: Envia as alterações de senha para o backend e atualiza a senha da conta.

### Fluxo de Navegação
- **Editar Perfil**: Usuário altera informações pessoais -> Envia as alterações -> Dados são processados e atualizados -> Mensagem de sucesso ou erro é exibida.
- **Alterar Senha**: Usuário preenche os campos de senha -> Envia as alterações -> Senha é atualizada e uma mensagem de confirmação ou erro é exibida.

## 5. Funcionalidades Interativas
### Formulários
- **Edição de Perfil**: Campos para inserir nome e email, com validação para garantir dados corretos.
- **Alterar Senha**: Campos para inserir senha atual, nova senha e confirmação da nova senha, com validação para garantir a segurança.

### Componentes Dinâmicos
- **Histórico de Atividades**: Atualiza dinamicamente com base nas atividades recentes do usuário.
- **Mensagens de Sucesso/Error**: Atualizam dinamicamente com base na resposta do backend após o envio dos formulários.

## 6. Requisitos de Backend
### Endpoints de API
- **GET /profile**: Recupera as informações do perfil do usuário.
- **PUT /profile**: Atualiza as informações do perfil do usuário.
- **PUT /profile/password**: Atualiza a senha da conta do usuário.

### Dados Enviados e Recebidos
- **Editar Perfil**:
  - Enviados: Nome, Email
  - Recebidos: Confirmação de sucesso ou mensagem de erro
- **Alterar Senha**:
  - Enviados: Senha Atual, Nova Senha
  - Recebidos: Confirmação de sucesso ou mensagem de erro
- **Histórico de Atividades**:
  - Recebidos: Dados sobre as atividades recentes do usuário

## 7. Testes
### Casos de Teste
- **Visualização de Perfil**: Verificar se as informações do perfil são exibidas corretamente.
- **Edição de Perfil**: Testar a atualização das informações do perfil e verificar se as mudanças são salvas corretamente.
- **Alterar Senha**: Testar a alteração de senha e garantir que a nova senha seja aplicada corretamente.
- **Histórico de Atividades**: Verificar se o histórico de atividades é exibido corretamente e atualizado com as informações recentes.

### Critérios de Aceitação
- **Perfil do Usuário**: As informações do perfil devem ser exibidas e atualizadas corretamente.
- **Edição de Perfil**: As alterações no perfil devem ser salvas e refletidas corretamente.
- **Alterar Senha**: A senha deve ser alterada com sucesso e a nova senha deve ser aplicada.
- **Histórico de Atividades**: O histórico de atividades deve ser preciso e atualizado conforme as atividades recentes do usuário.

## 8. Anotações Adicionais
- Garantir que a experiência de usuário na tela de perfil seja intuitiva e que as informações sejam facilmente acessíveis e atualizáveis.
- Considerar a implementação de medidas de segurança adicionais para proteger as informações pessoais e a senha do usuário.

