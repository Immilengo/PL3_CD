# Dicionário de dados — Banco Palanca, cartões de crédito

> **Dados sintéticos.** O Banco Palanca é fictício. Os dados foram gerados por computador (`gerar_banco_palanca.py`, semente 2026) e seguem a estrutura do conjunto público *Default of Credit Card Clients* (Yeh & Lien, 2009, UCI), usado no curso de Klosterman, *Data Science Projects with Python*. Os montantes estão em kwanzas e as províncias são angolanas, mas nenhuma linha corresponde a uma pessoa real.

**Ficheiro:** `banco_palanca_cartoes.xlsx` (ou `.csv`) — 30 000 linhas × 26 colunas, uma linha por conta de cartão de crédito.
**Período:** últimos seis meses, de Abril (mês 6) a Setembro (mês 1).
**Pergunta do cliente:** *esta conta vai entrar em incumprimento no próximo mês?*

| Coluna | Significado | Valores |
|---|---|---|
| `ID` | Identificador da conta | texto, ex.: `927dd27f-1a76` |
| `LIMITE_CREDITO` | Limite de crédito do cartão (Kz) | 100 000 a 8 000 000 |
| `SEXO` | Sexo do titular | 1 = masculino; 2 = feminino |
| `ESCOLARIDADE` | Nível de escolaridade | 1 = pós-graduação; 2 = licenciatura; 3 = ensino secundário; 4 = outros |
| `ESTADO_CIVIL` | Estado civil | 1 = casado(a); 2 = solteiro(a); 3 = outros (união de facto, divorciado(a), viúvo(a)) |
| `IDADE` | Idade do titular (anos) | 21 a 75 |
| `PROVINCIA` | Província de residência | nome da província |
| `PAG_1` … `PAG_6` | Estado do pagamento no mês 1 (Setembro) … mês 6 (Abril) | −1 = pagou na totalidade; 1 = 1 mês de atraso; 2 = 2 meses; … 8 = 8 meses; 9 = 9 ou mais meses |
| `FACTURA_1` … `FACTURA_6` | Valor da factura do mês (Kz) | |
| `PAGO_1` … `PAGO_6` | Valor pago no mês (Kz) | |
| `INCUMPRIMENTO` | **Variável resposta:** a conta entrou em incumprimento no mês seguinte (Outubro)? | 1 = sim; 0 = não |

