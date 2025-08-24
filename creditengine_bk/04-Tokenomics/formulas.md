# Fórmulas e políticas (v0.1)
Juros simples aproximado por período: I = P * (rate_bps / 10_000) * (dias/360).
Mora diária: mora = saldo_em_atraso * mora_bps_daily/10_000 * dias_atraso.
Prova de reservas: raiz Merkle publicada e assinada; auditoria periódica; atualização em janela fixa.
Liquidação (colateral cripto): se LTV > ltv_max_bps, liquidar fração necessária com bônus de `liq_bonus_bps` ao comprador de liquidação.
