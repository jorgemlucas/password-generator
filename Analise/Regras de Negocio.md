# Regras de Negócio do Projeto Password Generator

- RN1 - Objetivo do Sistema: o sistema deve gerar senhas aleatórias e seguras para o usuário, permitindo personalização por tipo de caractere e tamanho, e fornecendo feedback sobre a força da senha.

- RN2 - Requisitos de Geração de Senha:
  - o usuário deve poder selecionar o tamanho da senha entre 4 e 64 caracteres;
  - o usuário deve poder ativar ou desativar os seguintes tipos de caracteres: letras maiúsculas, letras minúsculas, números e caracteres especiais;
  - a geração de senha só deve ocorrer se pelo menos um tipo de caractere estiver selecionado;
  - cada senha gerada deve ter o número de caracteres exato escolhido pelo usuário;
  - a senha deve ser composta apenas pelos caracteres permitidos nas opções selecionadas.

- RN3 - Avaliação de Força da Senha:
  - deve existir um indicador de força que avalie se a senha é fraca, média ou forte;
  - o sistema deve alertar o usuário quando a senha for fraca, por exemplo quando o tamanho for menor que 8 caracteres ou quando apenas um tipo de caractere estiver selecionado.

- RN4 - Histórico de Senhas:
  - o sistema deve armazenar em memória até 5 senhas geradas recentemente durante a sessão;
  - o histórico não deve persistir após o fechamento da aba ou do navegador;
  - o usuário deve poder limpar manualmente o histórico de senhas a qualquer momento.

- RN5 - Usabilidade e Experiência:
  - deve haver um botão para copiar a senha gerada para a área de transferência;
  - o sistema deve exibir mensagens de erro ou alerta claras, por exemplo quando nenhuma opção de caractere está selecionada;
  - a interface deve ser responsiva e usável em diferentes tamanhos de tela.

- RN6 - Preferência de Tema:
  - o usuário deve poder alternar entre tema claro e escuro;
  - a preferência de tema deve ser salva no localStorage para ser mantida entre visitas.

- RN7 - Segurança:
  - a geração de senhas deve usar uma fonte de aleatoriedade segura, preferencialmente a API Web Crypto (crypto.getRandomValues);
  - o projeto deve evitar o uso de Math.random() para a geração final das senhas;
  - não deve haver persistência de senhas geradas no navegador além do histórico de sessão.

- RN8 - Validações e Restrições:
  - não permitir geração de senha se nenhum dos tipos de caractere estiver selecionado;
  - a senha deve ser gerada apenas quando o usuário solicitar explicitamente a ação ou quando as opções forem atualizadas com validação;
  - a interface deve habilitar ou desabilitar controles de acordo com o estado das seleções e exibir mensagem de erro apropriada.

- RN9 - Testes e Qualidade:
  - deve existir uma forma de validar as funcionalidades principais do gerador, como em tests.html;
  - os testes devem cobrir pelo menos: tamanho da senha, uso correto dos conjuntos de caracteres selecionados, comportamento quando nenhuma opção está selecionada, geração de senhas diferentes a cada chamada, persistência de tema no localStorage e limpeza de histórico de senhas.

- RN10 - Limitações do Sistema:
  - o histórico de senhas deve ser volátil e não persistir fora da sessão ativa;
  - o projeto não deve armazenar ou transmitir senhas geradas para servidores externos;
  - a força da senha é uma estimativa baseada em tamanho e variedade de caracteres, e não garante proteção contra todos os ataques.
