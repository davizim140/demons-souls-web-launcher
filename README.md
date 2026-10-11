# Demon's Souls Web Launcher

Projeto experimental para testar recursos do navegador antes de investigar uma possível execução de Demon’s Souls (PS3) em ambiente web.

## Estado atual

Esta primeira fase é um **launcher de diagnóstico**, não um emulador. A página testa WebGPU, WebAssembly, alguns recursos de threads e permite selecionar arquivos locais para conferir nome/tamanho. Os arquivos não são enviados para um servidor.

## Publicar gratuitamente com GitHub Pages

1. Abra **Settings → Pages** neste repositório.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Escolha a branch `main` e a pasta `/ (root)`, depois salve.
4. Aguarde a publicação e abra o endereço exibido na página Pages.

O workflow em `.github/workflows/pages.yml` também configura publicação automática pelo GitHub Actions. Se preferir usá-lo, em **Settings → Pages**, selecione **GitHub Actions** como origem de build/deploy.

## Limites importantes

- Não há emulador PS3 incluído ou integrado.
- O teste de WebGPU/WebAssembly não prova que o computador consegue emular um PS3.
- Selecionar um arquivo não verifica a integridade, a procedência ou a compatibilidade dele.
- Para uma futura integração, será necessário avaliar um emulador com suporte real a navegador/WASM, licenças, requisitos de firmware e compatibilidade específica do jogo.
- Use apenas cópias de jogos e firmware que você tenha direito de utilizar. Este projeto não distribui conteúdo de jogo, firmware ou chaves.

## Desenvolvimento

É uma página estática: abra `index.html` em um navegador moderno. Alguns recursos, como WebGPU, podem exigir HTTPS e suporte específico do navegador/driver.
