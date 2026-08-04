# Dúvidas e Lacunas do Projeto password-generator

## 1. Requisitos Funcionais
- O gerador deve permitir selecionar o tamanho da senha? Qual o intervalo mínimo e máximo?
- Deve suportar letras maiúsculas, minúsculas, números e símbolos especiais?
- Deve haver opções de exclusão de caracteres similares (como `l`, `1`, `O`, `0`)?
- O gerador precisa salvar senhas no navegador/usuário ou apenas mostrar/copiar?
- Existem regras específicas para força de senha ou validação?

## 2. Experiência do Usuário
- Há uma interface esperada para exibir a senha gerada e permitir cópia direta?
- Deve existir feedback visual se a senha gerada é considerada fraca, média ou forte?
- Como o usuário escolhe os parâmetros da senha (checkboxes, sliders, campos de texto)?
- O projeto precisa ser responsivo para dispositivos móveis?

## 3. Segurança
- Há necessidade de usar geração criptograficamente segura (`crypto.getRandomValues`) em vez de `Math.random()`?
- Como o projeto deve lidar com geração em ambientes offline e navegadores antigos?
- Deveria haver uma explicação sobre limitações de segurança no `README`?

## 4. Código e Estrutura
- O projeto deve ter arquivos JavaScript/CSS externos em vez de scripts internos no HTML?
- Existe a intenção de adicionar testes automatizados para as regras de senha?
- Há dependências externas planejadas ou o projeto deve ser 100% vanilla?
- O README atual descreve claramente como usar o gerador e como testar?

## 5. Documentação e Testes
- O `README.md` inclui exemplos de uso e instruções de execução?
- O `tests.html` cobre casos relevantes de uso ou é apenas um protótipo manual?
- Há planos para criar uma suite de testes automatizados (por exemplo, com Jest ou Cypress)?

## 6. Lacunas Prováveis
- Falta de descrição clara dos requisitos do gerador no `README`.
- Possível ausência de validação de parâmetros de entrada para tamanho e tipos de caractere.
- Falta de acessibilidade e usabilidade em dispositivos móveis.
- Ausência de testes automatizados ou de documentação de como um usuário deve validar o funcionamento.

## 7. Próximos Passos Sugeridos
- Revisar o conteúdo de `README.md`, `index.html` e `tests.html` para identificar requisitos implícitos.
- Definir claramente as funcionalidades desejadas e o fluxo do usuário.
- Adicionar documentação técnica ou de uso para reduzir dúvidas.
- Criar testes automatizados com base nos cenários mais importantes.
