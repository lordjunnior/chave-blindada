# chave-blindada

> Sistema de blindagem de chaves e assinatura por limiar (FROST): proteja seu patrimônio eliminando o ponto único de falha, sem que nenhum aparelho isolado tenha o poder de gastar seu saldo.

---

## Proposta

Guardar uma chave privada inteira em um único computador, celular ou anotada em um papel cria uma fragilidade crítica: quem encontrar ou invadir aquele ponto específico leva todo o seu dinheiro.

O projeto **chave-blindada** ensina a estruturar uma fortaleza criptográfica onde o poder de movimentação é blindado por regras matemáticas (FROST / Threshold Signatures), mantendo a custódia 100% nas suas mãos:

* **Imunidade contra invasões:** A chave mestra completa nunca fica gravada em nenhum dispositivo. Ela opera por fragmentos matemáticos isolados.
* **Aprovação soberana (Regra M de N):** Uma transação só sai se você autorizar em dois ou mais aparelhos pessoais previamente definidos (por exemplo: computador de casa + celular pessoal).
* **Zero rastro público:** Para o resto do mundo e para a blockchain, a transação parece uma operação comum de chave única, economizando taxas e preservando sua privacidade.
* **Isolamento de memória (Enclaves):** Os módulos de segurança rodam em ambientes blindados do sistema operacional, impedindo que vírus ou programas espiões leiam os dados.

---

## Estrutura do Repositório

```text
chave-blindada/
├── README.md
├── LICENSE
└── manuais/
    ├── 01-fundamentos-e-assinatura-blindada.md
    ├── 02-cerimonia-de-criacao-dkg.md
    ├── 03-enclaves-e-blindagem-de-memoria.md
    ├── 04-regras-de-autorizacao-e-quorom.md
    ├── 05-comunicacao-cifrada-e-assinatura-remota.md
    └── 06-auditoria-local-e-recuperacao.md