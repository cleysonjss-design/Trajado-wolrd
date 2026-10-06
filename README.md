# Trajado World — protótipo multiplayer

Protótipo em Godot 4 para um mundo aberto 3D com:
- lobby/sala
- até 30 jogadores
- servidor ENet
- mapa 3D com prédios
- personagem 3D
- movimentação WASD e pulo
- estrutura preparada para expandir para veículos, inventário, armas e modos de jogo

## Como abrir
1. Instale Godot 4.x.
2. Importe a pasta deste projeto.
3. Execute `main.tscn`.

## Multiplayer
O protótipo usa ENet na porta 7777. Para jogar pela internet, o servidor precisa ser executado em uma máquina/VM com a porta UDP 7777 liberada. Para uma versão pública, recomendamos servidor dedicado e autenticação.

## Observação
Este é um protótipo inicial, não uma cópia de Roblox/Free Fire e não inclui assets proprietários dessas marcas.
