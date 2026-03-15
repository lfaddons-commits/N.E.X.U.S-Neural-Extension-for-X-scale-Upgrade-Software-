​🌌 N.E.X.U.S. - Neon Protocol
​N.E.X.U.S. (Neural Extension for X-scale Upgrade Software) é um jogo de sobrevivência roguelike minimalista com estética Neon, desenvolvido em JavaScript puro e HTML5 Canvas. Focado em alta performance para dispositivos móveis e extensibilidade total via mods.
​🚀 Sobre o Jogo
​Em um sistema digital infestado por códigos corrompidos, você controla uma unidade de elite que evolui em tempo real. O objetivo é sobreviver a ondas de inimigos, coletar dados (XP) e injetar novos protocolos (Upgrades) no seu núcleo.
​Diferenciais:
​Engine Própria (Neon Engine): Leve, rápida e otimizada para navegadores mobile.
​Modding Nativo: Sistema de Registry e ModAPI que permite alterar quase tudo no jogo sem mexer no código fonte.
​Interface Mobile-First: Joystick virtual responsivo e menus adaptados para touch.
​🛠 Estrutura para Modders
​O N.E.X.U.S. foi construído sobre o NeonCore Framework, uma biblioteca de suporte que facilita a criação de conteúdo:
​Registry: Sistema central para registrar novos inimigos, habilidades e biomas.
​Event Driven: Hooks de eventos como gameTick, playerDamage e modLoaded.
​Asset Library: Banco de sons, cores neon e fórmulas de raridade pré-configuradas.
​Como instalar Mods:
​Abra o Mod Hub dentro do jogo.
​Selecione um arquivo .js do seu dispositivo ou insira uma URL externa.
​O sistema injetará o código em tempo real via FileReader ou eval.
​🏗 Como contribuir
​Se você é um desenvolvedor ou criador de mods:
​Faça um Fork deste repositório.
​Crie sua branch (git checkout -b feature/MeuMod).
​Desenvolva seu mod utilizando a ModAPI.
​Abra um Pull Request.
​📜 Licença
​Distribuído sob a licença MIT. Veja LICENSE para mais informações.

 Exemplo de Mod Rápido (API)
 // Criando um novo inimigo "Fantasma" com 1 linha usando NeonCore
ModAPI.registerEnemy('ghost_mod', {
    ...NeonCore.Templates.Enemies.Ghost,
    hp: 25,
    speed: 150
});

NeonCore.notify("Protocolo Ghost Ativado!", NeonCore.Palette.ICE);
