# Viraliza Vendas — projeto Android

## O que esta versão inicial faz
- Abre como aplicativo Android em tela cheia.
- Permite selecionar uma foto do produto.
- Cria prompts UGC em português para usar no Google Flow.
- Copia o prompt e abre o Google Flow.
- Guarda os prompts recentes localmente no aparelho.

## Como gerar o APK
1. Instale o Android Studio em um computador.
2. Abra a pasta `ViralizaVendasAndroid` no Android Studio.
3. Aguarde a sincronização do Gradle.
4. Se necessário, instale o Android SDK 35 pelo SDK Manager.
5. Use **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. O APK de teste será criado em `app/build/outputs/apk/debug/app-debug.apk`.

## Limitações desta versão
Esta é uma primeira versão funcional de interface e criação de prompts. Ela não gera vídeos diretamente: abre o Google Flow para a geração, que depende da conta e dos créditos disponíveis. O histórico fica salvo localmente no aparelho. Não há publicação na Play Store nem serviço de nuvem nesta versão.

## Compilação automática na nuvem (sem Android Studio)
1. Crie uma conta no GitHub e um repositório novo.
2. Envie todos os arquivos e pastas deste projeto para o repositório.
3. Abra a aba **Actions** do repositório.
4. Escolha **Build Android APK** e toque em **Run workflow**.
5. Quando terminar, abra a execução concluída e baixe o artefato **ViralizaVendas-APK**.
6. Extraia o arquivo ZIP baixado para encontrar `app-debug.apk` e transfira-o para o Android.

O APK gerado por esse fluxo é uma versão de depuração para testes. Para distribuir amplamente, será necessário configurar assinatura de release.
