# Trajado World — pacote Android

Este pacote contém o projeto Godot e uma automação para gerar o APK Android no GitHub Actions.

## Importante
Eu não consigo anexar um APK compilado diretamente deste ambiente porque o build Android precisa do ambiente/export templates do Godot. O pacote já está preparado para o GitHub Actions fazer essa compilação automaticamente.

## Como gerar o APK
1. Crie um repositório no GitHub.
2. Envie TODOS os arquivos desta pasta.
3. No GitHub, abra **Actions**.
4. Execute **Build Android APK** em **Run workflow**.
5. Ao terminar, baixe o artefato **TrajadoWorld-Android**.
6. Se você criar uma tag `v0.1.0`, o workflow também cria uma Release com o APK.

A automação usa Godot 4.7.2 e o exportador `firebelley/godot-export`, cuja documentação informa suporte a builds Android e requer um `export_presets.cfg`. 

## Onde hospedar para os amigos
Opção simples: GitHub Releases. Publique o APK como Release e envie o link da Release para os 30 amigos.

Outra opção: Cloudflare Pages para uma página de download. O Pages aceita upload direto de arquivos/ZIP e serve o conteúdo em um endereço `pages.dev`.

## Servidor multiplayer
O APK não é o servidor. Para 30 jogadores pela internet, será necessário um servidor dedicado com a porta UDP 7777 liberada. O protótipo atual contém a base ENet, mas ainda precisa de uma etapa de rede/autoridade de servidor antes de ser considerado pronto para uma partida real com 30 pessoas.

## Controles
A versão atual do projeto ainda é uma base de gameplay. Para a versão Android final, a próxima etapa é trocar os controles de teclado por joystick/botões touch e colocar câmera de terceira pessoa.
