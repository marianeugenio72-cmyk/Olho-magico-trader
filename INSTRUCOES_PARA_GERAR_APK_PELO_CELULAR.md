# Como gerar o APK pelo celular usando GitHub + Codemagic

Você não precisa de notebook.

## 1. Crie uma conta no GitHub
Entre no site do GitHub pelo navegador do celular e crie uma conta.

## 2. Crie um repositório novo
Nome sugerido:

`olho-magico-trader`

Deixe como privado ou público.

## 3. Envie os arquivos
Envie todos os arquivos desta pasta para o repositório:
- lib
- pubspec.yaml
- analysis_options.yaml
- README.md
- codemagic.yaml

## 4. Entre no Codemagic
Crie conta no Codemagic e conecte com o GitHub.

## 5. Escolha o projeto
Selecione o repositório `olho-magico-trader`.

O Codemagic vai encontrar o arquivo `codemagic.yaml`.

## 6. Rode o build
Escolha o workflow:

`Gerar APK Android`

Clique em iniciar build.

## 7. Baixe o APK
Quando terminar, vá em Artifacts e baixe:

`app-release.apk`

Esse é o arquivo que você instala no Android.

## Observação importante
Na primeira instalação, o Android pode pedir para permitir instalação de fontes desconhecidas.
Ative somente se você confiar no APK gerado por você.

## Se der erro
O erro mais comum é o projeto não ter a pasta Android ainda. Este pacote já manda o Codemagic rodar:

`flutter create .`

Isso cria a parte Android automaticamente.
