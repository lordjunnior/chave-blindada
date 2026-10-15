---
titulo: "Regras de Autorizacao e Quorum (Politicas M de N)"
descricao: "Como desenhar a matriz de seguranca ideal para o seu perfil de risco combinando multiplos dispositivos."
---

# Regras de Autorizacao e Quorum: A Matriz de Seguranca

A grande vantagem da arquitetura de limiar e a flexibilidade. Voce nao esta preso a uma regra rigida: voce define exatamente quantas pecas compoem o seu tabuleiro de seguranca.

---

## 1. A Notacao M de N

Nas politicas de controle, utilizamos a formula padrao **M de N**:
* **N** representa o numero total de fragmentos (aparelhos) criados na cerimonia.
* **M** representa o numero minimo de fragmentos necessarios para assinar e liberar qualquer transacao.

Exemplos de configuracao comuns:

### Configuracao 1 de 2 (Alta Disponibilidade com Alerta)
* Nao recomendado para cofres principais de longo prazo, mas util para operacoes corriqueiras onde qualquer um dos dois aparelhos pode movimentar sozinho, servindo como redundancia.

### Configuracao 2 de 2 (Seguranca Absoluta Contra Roubo Fisico)
* Exige a participacao simultanea de ambos os aparelhos. 
* Se um ladrao roubar o seu celular na rua, ele nao consegue roubar seus bitcoins porque o fragmento complementar esta seguro em casa no seu computador.
* *Risco:* Se voce perder permanentemente qualquer um dos dois aparelhos sem backup, os fundos ficam travados para sempre.

### Configuracao 2 de 3 (O Equilibrio Otimo)
* Voce possui 3 aparelhos com fatias diferentes. Qualquer combinacao de 2 aprova o gasto.
* Permite perder ou quebrar um aparelho inteiro sem perder o acesso aos fundos, mantendo forte protecao contra invasores solitarios.

---

## 2. Definindo Politicas por Faixa de Valor

Sistemas avancados de custodia permitem criar regras dinamicas baseadas no tamanho da saida financeira:
* **transacoes menores (Gastos diarios):** Podem exigir apenas uma autorizacao local simples.
* **transacoes pesadas (Reserva de valor):** Exigem obrigatoriamente o quórum completo de 2 ou 3 dispositivos distribuidos geograficamente.