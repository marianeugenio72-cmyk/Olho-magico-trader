# Olho Mágico Trader — MVP Android Flutter

App Android Flutter para ler candles em tempo real de **Binance** e base para **Deriv**, com motor técnico M1/M5 para gerar sinais:

- CALL
- PUT
- AGUARDAR

## Importante

Este app é um MVP de análise e sinais. Ele **não garante 99% de acerto**, não é recomendação financeira e não executa ordens com dinheiro real. Use primeiro em conta demo e faça backtest.

## Como rodar

1. Instale Flutter: https://docs.flutter.dev/get-started/install
2. Abra esta pasta no Android Studio ou VS Code.
3. Rode:

```bash
flutter pub get
flutter run
```

## O que já vem pronto

- Tela Android com seletor de fonte: Binance ou Deriv Demo.
- Timeframe M1 ou M5.
- Campo de ativo.
- WebSocket Binance para candles reais.
- WebSocket Deriv com exemplo de subscribe de candles.
- Motor de sinal com:
  - tendência por EMA 9/21
  - RSI
  - força de candle
  - pavio/rejeição
  - lateralização
  - volatilidade
  - suporte/resistência simples
- Score de confiança.
- Bloqueio de entrada quando o mercado está ruim.

## Ativos exemplo

### Binance
Use símbolos em minúsculo:
- btcusdt
- ethusdt
- solusdt

### Deriv
Símbolos comuns:
- R_100
- R_75
- R_50
- R_25

## Próximos passos profissionais

1. Fazer backtest com 50 mil+ candles.
2. Salvar sinais e resultados em banco local.
3. Criar painel de estatística.
4. Ligar API autenticada apenas depois de validar em demo.
5. Criar proteção de banca: stop diário, limite de perda, trava de horário.
