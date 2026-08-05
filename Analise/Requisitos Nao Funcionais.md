# Requisitos Não Funcionais do Projeto Password Generator

## RNF01 - Usabilidade
- A interface deve ser intuitiva e fácil de usar para usuários com conhecimento básico em informática.
- Os controles devem ser legíveis e de fácil acesso em telas de diferentes tamanhos.
- O sistema deve fornecer feedback claro para ações do usuário, como cópia de senha e erros de validação.

## RNF02 - Performance
- A geração de senha deve ocorrer instantaneamente ao usuário solicitar a operação.
- A interface deve responder rapidamente às alterações de configuração, como mudança de tamanho e seleção de caracteres.

## RNF03 - Compatibilidade
- O projeto deve funcionar corretamente em navegadores modernos como Chrome, Firefox, Edge e Safari.
- O sistema deve manter funcionalidade básica em dispositivos desktop e móveis.

## RNF04 - Segurança
- A geração de senha deve utilizar uma fonte de aleatoriedade segura, como a API Web Crypto (`crypto.getRandomValues`).
- O sistema não deve armazenar senhas geradas de forma persistente no navegador.
- As senhas não devem ser enviadas para servidores externos.

## RNF05 - Confiabilidade
- O histórico de senhas em memória deve manter até 5 entradas corretamente sem perda de dados durante a sessão.
- O sistema deve tratar corretamente estados inválidos, como tentativa de gerar senha com nenhum tipo de caractere selecionado.

## RNF06 - Manutenibilidade
- O código deve ser organizado de forma clara para facilitar atualizações futuras no gerador de senhas.
- A documentação do projeto deve estar disponível para facilitar entendimento de funcionalidades e requisitos.

## RNF07 - Acessibilidade
- O projeto deve fornecer contraste adequado entre texto e plano de fundo para facilitar a leitura.
- Os controles devem ser acessíveis para navegação por teclado e leitura de tela quando possível.

## RNF08 - Portabilidade
- O sistema deve ser facilmente executável localmente sem necessidade de servidores, bastando abrir `index.html`.
- O projeto deve ser construído com tecnologias web padrão (HTML, CSS e JavaScript) sem dependências externas pesadas.

## RNF09 - Escalabilidade (aplicável ao contexto do projeto)
- A estrutura do projeto deve permitir inclusão futura de novos tipos de caracteres ou indicadores de força.
- O layout e a arquitetura devem suportar expansão com novos controles e funcionalidades sem reescrita completa.
