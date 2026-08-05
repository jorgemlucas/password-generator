# Casos de Uso dos Requisitos Funcionais

## Caso de Uso 1 - Gerar Senha Personalizada
- Ator: Usuário
- Requisitos relacionados: RF01, RF04, RF07
- Pré-condição: O usuário acessa a página do gerador de senhas.
- Fluxo principal:
  1. O usuário define o tamanho da senha.
  2. O usuário seleciona os tipos de caracteres desejados (maiúsculas, minúsculas, números, especiais).
  3. O usuário clica em "Gerar Nova Senha".
  4. O sistema gera uma senha aleatória de acordo com as seleções.
  5. O sistema exibe a senha gerada.
- Pós-condição: A senha é exibida no campo de resultado.
- Exceção: Se nenhum tipo de caractere for selecionado, o sistema exibirá mensagem de erro e não gerará a senha.

## Caso de Uso 2 - Verificar Força da Senha
- Ator: Usuário
- Requisitos relacionados: RF02
- Pré-condição: Uma senha foi gerada.
- Fluxo principal:
  1. O sistema avalia a senha gerada.
  2. O sistema atribui um nível de força à senha: fraca, média ou forte.
  3. O sistema exibe o indicador de força.
- Pós-condição: O usuário visualiza se a senha é forte o suficiente.
- Exceção: Se a senha for fraca, o sistema destaca o alerta de segurança.

## Caso de Uso 3 - Copiar Senha para a Área de Transferência
- Ator: Usuário
- Requisitos relacionados: RF03
- Pré-condição: Uma senha foi gerada e exibida.
- Fluxo principal:
  1. O usuário clica no botão de copiar.
  2. O sistema copia a senha para a área de transferência.
  3. O sistema exibe confirmação visual de que a senha foi copiada.
- Pós-condição: A senha está disponível para colagem em outros serviços.

## Caso de Uso 4 - Consultar Histórico de Senhas Geradas
- Ator: Usuário
- Requisitos relacionados: RF05
- Pré-condição: Ao menos uma senha foi gerada na sessão.
- Fluxo principal:
  1. O usuário visualiza a seção de histórico de senhas.
  2. O sistema apresenta até as últimas 5 senhas geradas.
- Pós-condição: O usuário vê as senhas geradas recentemente.
- Exceção: Se não houver senhas no histórico, o sistema exibe uma mensagem indicando que não há histórico.

## Caso de Uso 5 - Limpar Histórico de Senhas
- Ator: Usuário
- Requisitos relacionados: RF05
- Pré-condição: O histórico possui pelo menos uma senha.
- Fluxo principal:
  1. O usuário clica no botão de limpar histórico.
  2. O sistema remove todas as entradas do histórico.
  3. O sistema exibe que o histórico está vazio.
- Pós-condição: O histórico não contém mais nenhuma senha.

## Caso de Uso 6 - Alternar Tema Claro/Escuro
- Ator: Usuário
- Requisitos relacionados: RF06
- Pré-condição: O usuário está na página do gerador de senhas.
- Fluxo principal:
  1. O usuário clica no botão de alternância de tema.
  2. O sistema aplica o tema escolhido imediatamente.
  3. O sistema salva a preferência no localStorage.
- Pós-condição: O tema permanece ativo em visitas futuras.

## Caso de Uso 7 - Receber Mensagem de Erro de Validação
- Ator: Usuário
- Requisitos relacionados: RF07
- Pré-condição: O usuário tenta gerar uma senha.
- Fluxo principal:
  1. O usuário não seleciona nenhum tipo de caractere.
  2. O usuário clica em "Gerar Nova Senha".
  3. O sistema valida as opções e detecta o erro.
  4. O sistema exibe uma mensagem explicando que pelo menos uma opção deve ser selecionada.
- Pós-condição: O usuário corrige as opções e tenta novamente.

## Caso de Uso 8 - Gerar Senha Rapidamente
- Ator: Usuário
- Requisitos relacionados: RF01, RF04
- Pré-condição: Parâmetros válidos selecionados.
- Fluxo principal:
  1. O usuário define os parâmetros de geração.
  2. O usuário solicita a geração da senha.
  3. O sistema realiza a geração imediatamente.
  4. O sistema exibe a senha gerada em poucos instantes.
- Pós-condição: O usuário obtém a senha sem demora.
