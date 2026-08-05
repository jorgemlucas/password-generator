# Critérios de Aceitação do Projeto Password Generator

## HU01 - Gerar senha personalizada
- O usuário pode selecionar o tamanho da senha.
- O usuário pode incluir ou excluir maiúsculas, minúsculas, números e caracteres especiais.
- A senha gerada respeita exatamente as opções de caracteres selecionadas.
- A senha gerada possui o tamanho escolhido pelo usuário.

## HU02 - Verificar a força da senha
- A interface mostra um indicador de força após a geração da senha.
- O indicador de força diferencia claramente entre fraca, média e forte.
- A avaliação de força considera comprimento e tipos de caracteres usados.

## HU03 - Copiar senha com facilidade
- Há um botão ou ação clara para copiar a senha gerada.
- Ao clicar, a senha é copiada para a área de transferência.
- O usuário recebe um feedback visual ou mensagem de confirmação após a cópia.

## HU04 - Usar histórico de senhas geradas
- O sistema exibe as últimas senhas geradas na sessão atual.
- O histórico mostra as senhas em ordem cronológica (mais recente primeiro).
- O usuário pode reutilizar uma senha a partir do histórico sem ter que gerar novamente.

## HU05 - Limpar o histórico de senhas
- Há um controle visível para limpar o histórico de senhas.
- Ao limpar, todas as entradas do histórico da sessão são removidas.
- O usuário recebe confirmação de que o histórico foi apagado.

## HU06 - Alternar tema claro/escuro
- Existe um botão ou interruptor para alternar entre os temas.
- A interface muda imediatamente entre tema claro e escuro.
- O tema selecionado é aplicado em todos os elementos principais da aplicação.

## HU07 - Manter tema preferido
- A aplicação salva a preferência de tema do usuário.
- Ao recarregar a página, o tema preferido é restaurado automaticamente.
- A preferência persiste entre visitas usando armazenamento local.

## HU08 - Receber mensagem de erro quando não há opções válidas
- Se nenhum tipo de caractere estiver selecionado, a geração de senha não ocorre.
- O usuário vê uma mensagem de erro clara explicando o problema.
- A mensagem indica que é necessário selecionar ao menos um tipo de caractere.

## HU09 - Ter geração rápida de senhas
- A senha é gerada imediatamente quando o usuário clica no botão.
- Não há atraso perceptível entre o clique e a apresentação da senha.
- A interface permanece responsiva durante a geração.

## HU10 - Usar a aplicação localmente
- O arquivo `index.html` abre no navegador sem necessidade de instalação.
- Todas as funcionalidades funcionam localmente a partir do arquivo HTML.
- Não é preciso servidor ou dependência externa para usar a aplicação básica.
