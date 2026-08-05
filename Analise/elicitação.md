# Script de Elicitação — Projeto Password Generator

Objetivo: coletar requisitos com stakeholders para definir de forma clara comportamento, limites e critérios de aceitação do gerador de senhas.

---

## Abertura (1–2 min)
- Apresentar-se brevemente e explicar o propósito da sessão.
- Confirmar tempo disponível e participantes.
- Validar expectativas sobre o que será entregue (requisitos funcionais, não funcionais, restrições, prioridades).

## Contexto do Sistema (2–3 min)
- Resumo do sistema: "Um gerador de senhas web que cria senhas aleatórias personalizáveis, com avaliação de força, histórico de sessão e opção de tema."
- Perguntar se existem exemplos de uso ou integração esperada.

## Perguntas Diretas de Elicitação (fluxo principal)
### Requisitos Funcionais
1. RF01 — Geração de Senhas
  - Quem usará o gerador? (perfil do usuário)
  - Qual o intervalo mínimo e máximo aceitável para o tamanho da senha? Existe padrão institucional?
  - Quais conjuntos de caracteres são obrigatórios ou opcionais?
  - Há regras de formatação obrigatórias (ex.: pelo menos uma letra maiúscula, um número)?
2. RF02 — Indicador de Força
  - Como deve ser a métrica de força? (tamanho + variedade de caracteres, entropia estimada, etc.)
  - Existem limites definidos para considerar uma senha "aceitável" em sistemas integrados?
3. RF03 — Cópia de Senha
  - A cópia para o clipboard é suficiente ou é necessário registro de eventos (logs) de ação?
4. RF04 — Controle de Parâmetros
  - O slider de tamanho com valores predefinidos é aceitável ou preferem entrada numérica direta?
5. RF05 — Histórico de Senhas
  - Historico em memória é suficiente? Há necessidade de persistência por usuário autenticado?
  - Qual o número máximo aceitável de entradas no histórico?
6. RF06 — Tema e Preferências
  - A preferência de tema deve ser persistida entre sessões (localStorage) ou por usuário (backend)?
7. RF07 — Validações e Mensagens
  - Como deve ser a mensagem de erro padrão quando nenhuma opção está selecionada?

### Requisitos Não-Funcionais (RNs)
1. RNF01 — Segurança
  - É obrigatório usar Web Crypto API para geração segura?
  - Existem políticas de conformidade (ex.: GDPR, políticas internas) sobre armazenamento ou transmissão de senhas geradas?
2. RNF02 — Performance
  - Qual o tempo máximo aceitável para geração e exibição da senha?
3. RNF03 — Compatibilidade
  - Quais navegadores e versões devem ser suportados?
4. RNF04 — Acessibilidade
  - Existem requisitos de acessibilidade (WCAG) mínimos a suportar?

## Cenários e Exemplos (prototipagem rápida)
- Solicitar que o participante descreva um cenário típico de uso (ex.: geração para conta bancária, senha temporária, etc.).
- Pedir exemplos de regras específicas (por exemplo, "senha para sistema X deve ter pelo menos 12 caracteres e 2 tipos de caracteres especiais").

## Restrições e Integrações
- Verificar se há necessidade de integração com outros sistemas (SSO, gerenciadores de senha corporativos).
- Identificar restrições legais ou políticas de TI.

## Critérios de Aceitação (para cada RF)
- RF01: Ao gerar com parâmetros válidos, senha exibida com tamanho exato e apenas caracteres permitidos.
- RF02: Indicador de força apresenta no mínimo os três níveis (Fraca/Média/Forte) e sinaliza fraca quando tamanho < 8 ou apenas um conjunto selecionado.
- RF03: Botão de copiar coloca texto no clipboard e exibe confirmação visual.
- RF05: Histórico mantém até 5 entradas na sessão e é limpo ao fechar a aba.

## Priorização
- Perguntar quais requisitos são "must-have", "should-have" e "nice-to-have".
- Registrar prioridades para RF01, RF02 e RF07 como críticas por padrão (sugerido), e resto como secundário.

## Riscos e Dúvidas
- Registrar preocupações sobre segurança (armazenamento, exposição em clipboard, logs).
- Levantar dúvida sobre necessidade de auditoria de uso.

## Encerramento (2 min)
- Recapitular decisões e próximos passos.
- Confirmar responsáveis por ações e prazos para entrega dos requisitos finais.
- Agradecer participação e informar como receberão o documento final.

---

## Anexo: Checklist rápido de tópicos cobertos
- [ ] Perfil do usuário
- [ ] Tamanho mínimo/máximo da senha
- [ ] Conjuntos de caracteres obrigatórios
- [ ] Regras adicionais de composição
- [ ] Persistência do histórico
- [ ] Uso de Web Crypto API
- [ ] Requisitos de compatibilidade e acessibilidade
- [ ] Critérios de aceitação claros

