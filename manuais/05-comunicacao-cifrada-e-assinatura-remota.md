---
titulo: "Comunicacao Cifrada e Assinatura Remota"
descricao: "Como conectar seus dispositivos fatiados de forma segura usando protocolos criptograficos e relays descentralizados (Nostr)."
---

# Comunicacao Cifrada e Assinatura Remota: Conectando os Pontos com Seguranca

Para que um cofre com chaves blindadas funcione na pratica, os aparelhos fatiados precisam conversar entre si para juntar as assinaturas parciais quando voce decidir fazer um pagamento.

Como esses aparelhos estao em locais diferentes, a comunicacao ocorre atraves de canais de relay descentralizados, blindados por criptografia de ponta a ponta (E2EE).

---

## 1. O Uso do Protocolo Nostr para Coordenacao

O protocolo Nostr (Notes and Other Stuff Transported by Relays) fornece a infraestrutura perfeita para essa comunicacao:
* Os relays Nostr funcionam apenas como caixas postais cegas e publicas.
* Eles recebem mensagens cifradas por chaves efêmeras, mas nao conseguem ler o conteudo, saber quem esta falando ou quem esta respondendo.
* Se um relay cair ou for censurado, basta apontar os agentes para outro relay publico ou privado na rede.

---

## 2. O Fluxo de Assinatura a Distancia

1. **Disparo do Pedido:** O computador principal cria a transacao parcial e publica um evento cifrado direcionado aos demais aparelhos guardiões.
2. **Notificacao Segura:** O seu celular pessoal recebe a notificacao em segundo plano, descriptografa o payload usando sua chave privada local e exibe os detalhes exatos do pagamento na tela.
3. **Aprovação Biométrica ou por Senha:** Voce confere o valor e o destinatario, entao autoriza usando sua senha ou biometria local.
4. **Retorno da Assinatura Parcial:** O celular calcula a fatia de assinatura de Schnorr e a envia de volta por canal cifrado ao solicitante.
5. **Consolidacao e Envio:** O solicitante junta as partes, monta a transacao final e a transmite para a rede Bitcoin.

---

## 3. Mitigacao de Ataques de Negacao de Servico (DoS)

Como os relays sao publicos, e fundamental proteger os agentes contra spam:
* Os aparelhos so aceitam solicitacoes de conexao originadas de chaves publicas previamente autorizadas na configuracao inicial do grupo.
* Mensagens com carimbos de data/hora (timestamps) invalidos ou fora de janela sao sumariamente descartadas.