# Regras de Negócio do Projeto Password Generator

## 1. Objetivo do Sistema
O sistema deve gerar senhas aleatórias e seguras para o usuário, permitindo personalização por tipo de caractere e tamanho, e fornecendo feedback sobre a força da senha.

## 2. Requisitos de Geração de Senha
- O usuário deve poder selecionar o tamanho da senha entre 4 e 64 caracteres.
- O usuário deve poder ativar ou desativar os seguintes tipos de caracteres:
  - Letras maiúsculas
  - Letras minúsculas
  - Números
  - Caracteres especiais
- A geração de senha só deve ocorrer se pelo menos um tipo de caractere estiver selecionado.
- Cada senha gerada deve ter o número de caracteres exato escolhido pelo usuário.
- A senha deve ser composta apenas pelos caracteres permitidos nas opções selecionadas.

## 3. Avaliação de Força da Senha
- Deve existir um indicador de força que avalie se a senha é:
  - Fraca
  - Média
  - Forte
- O sistema deve alertar o usuário quando a senha for fraca:
  - Tamanho menor que 8 caracteres
  - Apenas um tipo de caractere selecionado

## 4. Histórico de Senhas
- O sistema deve armazenar em memória até 5 senhas geradas recentemente durante a sessão.
- O histórico não deve persistir após o fechamento da aba ou do navegador.
- O usuário deve poder limpar manualmente o histórico de senhas a qualquer momento.

## 5. Usabilidade e Experiência
- Deve haver um botão para copiar a senha gerada para a área de transferência.
- O sistema deve exibir mensagens de erro ou alerta claras, por exemplo quando nenhuma opção de caractere está selecionada.
- A interface deve ser responsiva e usável em diferentes tamanhos de tela.

## 6. Preferência de Tema
- O usuário deve poder alternar entre tema claro e escuro.
- A preferência de tema deve ser salva no `localStorage` para ser mantida entre visitas.

## 7. Segurança
- A geração de senhas deve usar uma fonte de aleatoriedade segura, preferencialmente a API Web Crypto (`crypto.getRandomValues`).
- O projeto deve evitar o uso de `Math.random()` para a geração final das senhas.
- Não deve haver persistência de senhas geradas no navegador além do histórico de sessão.

## 8. Validações e Restrições
- Não permitir geração de senha se nenhum dos tipos de caractere estiver selecionado.
- A senha deve ser gerada apenas quando o usuário solicitar explicitamente a ação ou quando as opções forem atualizadas com validação.
- A interface deve habilitar ou desabilitar controles de acordo com o estado das seleções e exibir mensagem de erro apropriada.

## 9. Testes e Qualidade
- Deve existir uma forma de validar as funcionalidades principais do gerador, como em `tests.html`.
- Os testes devem cobrir pelo menos:
  - tamanho da senha
  - uso correto dos conjuntos de caracteres selecionados
  - comportamento quando nenhuma opção está selecionada
  - geração de senhas diferentes a cada chamada
  - persistência de tema no `localStorage`
  - limpeza de histórico de senhas

## 10. Limitações do Sistema
- O histórico de senhas deve ser volátil e não persistir fora da sessão ativa.
- O projeto não deve armazenar ou transmitir senhas geradas para servidores externos.
- A força da senha é uma estimativa baseada em tamanho e variedade de caracteres, e não garante proteção contra todos os ataques.
