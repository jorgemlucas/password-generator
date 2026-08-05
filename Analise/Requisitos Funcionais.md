# Requisitos Funcionais do Projeto Password Generator

## 1. Geração de Senhas
- O sistema deve gerar senhas aleatórias ao usuário.
- O usuário deve poder escolher o tamanho da senha entre 4 e 64 caracteres.
- O usuário deve poder selecionar quais tipos de caracteres incluir na senha:
  - Letras maiúsculas
  - Letras minúsculas
  - Números
  - Caracteres especiais
- A senha gerada deve conter apenas caracteres dos tipos selecionados.
- A geração de senha deve ser bloqueada se nenhuma opção de caractere estiver selecionada.
- Cada nova geração deve produzir uma senha diferente da anterior na mesma sessão, sempre que possível.

## 2. Indicador de Força da Senha
- O sistema deve exibir um indicador de força para a senha gerada.
- O indicador deve distinguir, no mínimo, três níveis: fraca, média e forte.
- O sistema deve exibir alerta visual quando a senha for considerada fraca.

## 3. Cópia de Senha
- O usuário deve poder copiar a senha gerada para a área de transferência com um botão.
- Após a cópia, deve haver um retorno visual confirmando que a senha foi copiada.

## 4. Controle de Parâmetros
- O usuário deve poder ajustar dinamicamente o tamanho da senha com um controle de slider ou equivalente.
- O valor atual do tamanho da senha deve estar visível e atualizado conforme o usuário altera o controle.
- O usuário deve poder marcar ou desmarcar as opções de conjuntos de caracteres.

## 5. Histórico de Senhas
- O sistema deve manter um histórico dos últimos 5 senhas geradas na sessão.
- O histórico não deve persistir depois que o usuário fechar a aba ou o navegador.
- O usuário deve poder limpar manualmente o histórico de senhas.

## 6. Tema e Preferências
- O sistema deve permitir alternar entre tema claro e tema escuro.
- A preferência de tema deve ser armazenada no localStorage e reaplicada em visitas futuras.

## 7. Validações e Mensagens de Erro
- O sistema deve mostrar uma mensagem de erro se o usuário tentar gerar senha sem selecionar nenhum tipo de caractere.
- O sistema deve validar o tamanho mínimo e máximo da senha antes da geração.
- O sistema deve impedir a geração de senha com parâmetros inválidos.

## 8. Compatibilidade e Uso
- O usuário deve poder usar o gerador abrindo o arquivo `index.html` em um navegador moderno.
- O sistema deve ser acessível e funcional em diferentes tamanhos de tela.

## 9. Testes
- O projeto deve incluir testes que verifiquem:
  - geração de senha com tamanho correto
  - geração de senhas apenas com o conjunto de caracteres selecionado
  - erro quando nenhuma opção de caractere estiver selecionada
  - geração de senhas diferentes em chamadas consecutivas
  - comportamento de histórico e limpeza de histórico
  - persistência e recuperação da preferência de tema
