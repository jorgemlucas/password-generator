# 🔐 Gerador de Senhas

[![HTML](https://img.shields.io/badge/HTML-5-orange)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS-3-blue)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

Um gerador de senhas seguro e intuitivo, desenvolvido como projeto do curso de Engenharia de Software com IA da FGV. Permite criar senhas fortes personalizadas com opções de caracteres, tamanho ajustável e indicador de força.

## 📋 Descrição

Este projeto é um gerador de senhas web-based que ajuda usuários a criar senhas seguras e aleatórias. A ferramenta é ideal para melhorar a segurança digital, oferecendo controle total sobre os tipos de caracteres incluídos e o comprimento da senha. Inclui também um histórico de senhas geradas e testes automatizados para validar a funcionalidade.

## ✨ Funcionalidades

- **Geração de Senhas Personalizáveis**: Escolha entre letras maiúsculas, minúsculas, números e caracteres especiais.
- **Controle de Tamanho**: Ajuste o comprimento da senha de 4 a 64 caracteres via slider.
- **Indicador de Força**: Avaliação visual da força da senha (Fraca, Média, Forte).
- **Histórico de Senhas em Memória**: Armazena até 5 senhas recentes durante a sessão, sem persistir no navegador.
- **Botão Limpar Histórico**: Permite apagar manualmente o histórico a qualquer momento.
- **Limpeza Automática de Histórico**: O histórico é removido ao fechar a aba ou o navegador.
- **Alternância de Tema**: Toggle escuro/claro com ícone de lua/sol e preferência salva no `localStorage`.
- **Alerta de Senha Fraca**: Barra vermelha exibe aviso automático quando a senha tem menos de 8 caracteres ou usa apenas um tipo de caractere.
- **Aleatoriedade Segura**: A geração de senha usa a API Web Crypto (`crypto.getRandomValues`) em vez de `Math.random` para melhorar a segurança.
- **Copiar para Clipboard**: Botão para copiar a senha gerada facilmente.
- **Validação de Opções**: Impede geração sem pelo menos um tipo de caractere selecionado.
- **Testes Automatizados**: Arquivo `tests.html` para validar funcionalidades com JavaScript puro.

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura da página web.
- **CSS3**: Estilização responsiva e moderna com gradientes e animações.
- **JavaScript (ES6)**: Lógica de geração de senhas, validação e interatividade.
- **Web Crypto API**: Geração de números aleatórios seguros para fortalecer a senha gerada.
- **GitHub Copilot**: Assistência na codificação e geração de ideias.

## 🚀 Como Usar

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/seu-usuario/password-generator.git
   cd password-generator
   ```

2. **Abra o arquivo principal**:
   - Abra `index.html` em qualquer navegador web moderno (Chrome, Firefox, Edge, etc.).

3. **Personalize e Gere**:
   - Ajuste o tamanho da senha com o slider.
   - Selecione os tipos de caracteres desejados (maiúsculas, minúsculas, números, especiais).
   - Clique em "Gerar Nova Senha" ou as opções se atualizam automaticamente.
   - Copie a senha usando o botão "Copiar".

4. **Visualize o Histórico**:
   - As senhas geradas aparecem na seção de histórico abaixo.

## 🧪 Como Executar os Testes

O projeto inclui um arquivo de testes `tests.html` que valida as funcionalidades principais usando JavaScript puro.

1. Abra `tests.html` em um navegador web.
2. Clique no botão "Executar Testes".
3. Os resultados aparecerão na página:
   - ✅ Verde para testes que passaram.
   - ❌ Vermelho para testes que falharam.

Os testes verificam:
- Tamanho correto da senha.
- Respeito às opções selecionadas (ex: só números).
- Erro quando nenhuma opção é selecionada.
- Geração de senhas diferentes a cada chamada.

## 🤖 Contribuição da IA Generativa (GitHub Copilot)

O GitHub Copilot desempenhou um papel fundamental no desenvolvimento deste projeto, acelerando a implementação e melhorando a qualidade do código:

- **Geração de Código Base**: Auxiliou na criação da estrutura HTML inicial, estilos CSS responsivos e lógica JavaScript para geração de senhas.
- **Ideias de Funcionalidades**: Sugeriu a implementação do indicador de força da senha, histórico de senhas e validações de entrada.
- **Otimização e Debugging**: Ajudou a refinar algoritmos, corrigir bugs e otimizar o código para melhor performance.
- **Testes Automatizados**: Inspirou a criação do arquivo de testes `tests.html`, incluindo funções de validação e exibição de resultados.
- **Melhorias de UX**: Propôs animações, transições e design responsivo para uma experiência de usuário aprimorada.

O uso do Copilot permitiu focar mais na lógica de negócio e design, enquanto a IA cuidava de tarefas repetitivas e sugeria boas práticas de desenvolvimento.

Para mim, foi uma experiência realmente enriquecedora, pois foi a primeira vez que utilizei uma IDE integrada a um agente de IA. Enfrentei algumas dificuldades ao longo do caminho, mas, depois de erros e acertos — e com a ajuda do próprio agente — as barreiras foram sendo superadas. Ao final do processo, ficou a satisfação de ter construído algo. É verdade que o resultado foi simples, até modesto se comparado aos projetos dos colegas, mas trouxe aprendizados valiosos e a sensação de estar participando de algo novo.

## 📄 Licença

Este projeto é parte do curso de Engenharia de Software com IA da FGV e está disponível sob a licença MIT.

## 👥 Contribuintes

- Desenvolvido como projeto acadêmico por Jorge Mello Lucas com apoio do GitHub Copilot.
