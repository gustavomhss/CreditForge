# Política de Oráculos (v0.1)
Fontes: Chainlink (primária), TWAP on-chain (secundária), fallback assinado off-chain.
TWAP: janela `twap_window_seconds` (default 900s), atualizações por bloco-alvo.
Circuit breakers: pausa swaps/liquidações se |preço_atual - TWAP| > X% (ex.: 10%) ou se fonte primária indisponível > N blocos.
Retomada: janela de estabilidade de M minutos e 3 leituras válidas consecutivas.
