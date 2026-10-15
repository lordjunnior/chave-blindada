---
titulo: "Auditoria Local e Rotina de Recuperacao"
descricao: "Como realizar testes periodicos de integridade, substituir aparelhos antigos e garantir a continuidade sucessoria."
---

# Auditoria Local e Rotina de Recuperacao: Manutencao da Fortaleza

Uma chave blindada nao e um sistema que voce configura e esquece em uma gaveta. Como envolve tecnologia, dispositivos eletronicos e midias fisicas, e necessaria uma rotina periodica de manutencao para garantir que tudo funcione perfeitamente no dia em que voce mais precisar.

---

## 1. Rotina de Auditoria Trimestral

A cada tres meses, execute os seguintes passos de verificacao:
1. **Teste de Conectividade entre Pares:** Inicie uma sessao de teste de assinatura parcial entre os aparelhos para garantir que as chaves de sessao e os relays continuam respondendo.
2. **Verificacao de Midias Fisicas:** Confirme se os backups fisicos dos fragmentos e metadados guardados em cartoes MicroSD ou papel continuam legiveis e livres de danos fisicos.
3. **Atualizacao de Software:** Confira se os binarios executados nos dispositivos estao atualizados com as ultimascorrecoes de seguranca do repositorio oficial.

---

## 2. Substituicao de um Aparelho Comprometido ou Quebrado

Se um dos seus aparelhos quebrar, for perdido ou sofrer suspeita de invasao, o sistema nao esta perdido (desde que voce ainda possua o quorum minimo operacional):
1. Inicie o protocolo de rotacao de chaves (Key Rotation).
2. Adicione um novo aparelho limpo ao grupo atraves de uma nova rodada de DKG parcial.
3. Revogue formalmente o identificador do aparelho antigo.
4. A chave publica principal permanece exatamente a mesma, o que significa que **seus enderecos de Bitcoin continuam validos e intocados**, mas o aparelho antigo perdeu completamente qualquer capacidade de interagir com o cofre.

---

## 3. Planejamento Sucessório (Heranca Segura)

Como dividir uma chave blindada entre herdeiros sem expor o patrimonio antes da hora?

* **Distribuicao de Fatias por Regra M de N:**
  * Voce pode estruturar um esquema onde os herdeiros possuem partes complementares.
  * Por exemplo, em um grupo 2 de 3, voce guarda duas fatias com voce em locais separados e entrega a terceira fatia lacrada junto a um testamento juridico ou advogado de confianca.
  * Nenhum herdeiro isolado consegue mexer no dinheiro, mas em caso de ausencia permanente, a combinacao das partes autorizadas garante o acesso a familia sem friccao e sem intermediarios centralizados.