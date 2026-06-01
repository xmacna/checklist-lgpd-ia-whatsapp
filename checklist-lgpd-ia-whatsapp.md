# Checklist LGPD para agente de IA no WhatsApp

Ultima revisao: 2026-06-01

Este checklist ajuda a revisar um agente de IA para WhatsApp antes de colocar em producao. Ele nao e parecer juridico.

## P0 - Antes de publicar

1. Finalidade documentada
   - Defina se o agente faz atendimento, qualificacao, vendas, suporte, cobranca, agendamento ou outro processo.
   - Liste quais dados entram, de onde vem e para onde vao.
   - Evite coletar dados que nao sejam necessarios para a finalidade.

2. Base legal por etapa
   - Registre a base legal para cada etapa relevante: primeiro contato, qualificacao, CRM/Painel Inteligente, follow-up e retencao.
   - Nao trate consentimento como base universal. Quando a base for consentimento, registre prova e retirada.

3. Transparencia no inicio da conversa
   - Informe qual empresa esta atendendo.
   - Explique a finalidade do atendimento.
   - Informe que dados podem ser usados para atendimento, qualificacao e melhoria do processo.
   - Ofereca caminho simples para falar com humano quando fizer sentido.

4. Minimizacao de dados
   - Colete apenas nome, contato, interesse e contexto comercial quando isso bastar.
   - Bloqueie perguntas que induzam envio de documentos, dados financeiros sensiveis, saude, biometria ou dados de criancas sem necessidade real.

5. Dados sensiveis
   - Se o processo puder receber dado sensivel, trate como fluxo de risco maior.
   - Crie regra de escalonamento humano e reducao de retencao.
   - Evite usar dado sensivel para segmentacao comercial.

6. Papeis e contratos
   - Defina quem e controlador e quem e operador.
   - Liste fornecedores: WhatsApp, CRM/Painel Inteligente, automacao, armazenamento, analytics e XMACNA quando aplicavel.
   - Garanta contrato, DPA ou clausulas de privacidade quando houver tratamento por operador.

7. Canal de direitos do titular
   - Tenha canal para confirmacao, acesso, correcao, exclusao, portabilidade quando aplicavel, informacao sobre compartilhamento e revisao de decisoes automatizadas.
   - Garanta que o time saiba reconhecer esses pedidos no WhatsApp.

8. Retencao e descarte
   - Defina prazo para leads sem resposta, leads desqualificados e clientes ativos.
   - Remova ou anonimiza conversas antigas quando nao houver finalidade ativa.

9. Seguranca
   - Use MFA nas contas administrativas.
   - Restrinja acesso por necessidade.
   - Proteja credenciais, chaves de acesso e URLs sensiveis.
   - Registre logs suficientes para auditoria sem expor dados desnecessarios.

10. Decisoes automatizadas
   - Se a IA pontua, qualifica ou prioriza leads, documente a regra geral.
   - Evite bloquear atendimento, credito, servico essencial ou direito apenas por decisao automatizada.
   - Ofereca revisao humana quando a decisao puder afetar direito ou interesse relevante.

11. Base de conhecimento e prompts
   - Nao coloque segredo, credencial ou dado pessoal desnecessario no prompt.
   - Revise documentos usados como contexto.
   - Teste se o agente inventa politicas, precos, promessas ou bases legais.

12. Evidencia operacional
   - Guarde versao do fluxo, prompt principal, bases de conhecimento e politicas de retencao.
   - Registre testes antes de publicar.
   - Para risco alto, prepare RIPD/relatorio de impacto com responsavel juridico ou DPO.

## Sinais de risco maior

- Dados de saude, criancas, biometria, geolocalizacao precisa ou documentos.
- Atendimento financeiro, medico, educacional sensivel ou juridico.
- Uso de IA para negar acesso, classificar risco, aprovar credito ou limitar servico.
- Compartilhamento com muitos fornecedores.
- Falta de canal claro para o titular.

## Fontes oficiais

As fontes oficiais usadas estao em `sources.md`.
