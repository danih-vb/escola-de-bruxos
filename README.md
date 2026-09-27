# Escola de Bruxos

Modpack "kitchen sink" para **Minecraft 1.7.10**, com foco em magia — vários sistemas mágicos
completos rodando lado a lado (Thaumcraft, Witchery, Botania, Blood Magic, Ars Magica 2, AbyssalCraft
e mais), além de exploração, tecnologia/automação, mobs e um sistema de comida completo.

Criado e mantido por Daniel Velluto Bento, testado e ajustado mod por mod pra rodar de forma
estável num servidor privado entre amigos.

- 📋 Lista completa de mods e changelog: [`MODLIST.md`](MODLIST.md)
- ⌨️ Atalhos customizados (o que foi remapeado e por quê, + referência completa de todos os
  atalhos do pack): [`KEYBINDS.md`](KEYBINDS.md)

## Requisitos
- **Minecraft**: 1.7.10
- **Forge**: 10.13.4.1614
- **Java**: 8 (obrigatório — o pack roda em código muito antigo e não é compatível com Java 17+)
- RAM recomendada: pelo menos 6 GB alocados ao Java (pack pesado, 186 mods)

## Estrutura do repositório
Este repositório é, na prática, a **pasta de jogo completa** do modpack — não só os mods, mas
tudo que o Forge e os mods precisam para rodar exatamente como no ambiente de testes. Ele foi
gerado a partir de um **perfil do TLauncher com "diretório de jogo separado" ativado** (por isso
`Hogwarts.jar` e `Hogwarts.json` — os arquivos da versão customizada — ficam na raiz, junto com
`mods/`, `config/`, `saves/` etc., em vez de dentro de uma pasta `.minecraft/versions/` separada).

```
Escola de Bruxos/
├── Hogwarts.jar / Hogwarts.json   ← arquivos da versão (Forge 1.7.10 já "instalado")
├── TLauncherAdditional.json       ← metadados específicos do TLauncher para essa versão
├── options.txt                    ← configurações de vídeo/som + atalhos (ver KEYBINDS.md)
├── localconfig.cfg                ← preferências salvas de alguns mods (ex.: NotEnoughItems)
├── BotaniaVars.dat                ← progresso/flags globais do Botania
├── knownkeys.txt                  ← cache interno de atalhos já vistos pelo Forge
├── README.md / MODLIST.md / KEYBINDS.md
│
├── mods/                          ← os 160 arquivos .jar/.zip dos 186 mods (ver MODLIST.md)
│   └── 1.7.10/                    ← alguns mods mais antigos (Baubles, CodeChickenLib etc.)
│
├── config/                        ← arquivo .cfg/.json de configuração de cada mod
│
├── resourcepacks/                 ← resource packs opcionais do jogador
├── resources/                     ← recursos próprios do modpack (texturas de GUI custom)
├── scripts/                       ← scripts do CraftTweaker (ex.: `projecte_default.zs`)
│
├── ambience_music/                ← trilhas do mod Ambience
├── fonts/                         ← fonte customizada usada por algum mod de HUD
│
├── saves/                         ← mundos locais (singleplayer) — dado pessoal, não obrigatório
├── backups/                       ← backups automáticos de mundo (AromaBackup) — dado pessoal
├── crash-reports/                 ← relatórios de crash — dado pessoal/temporário
├── logs/                          ← logs do jogo, incl. fml-client-latest.log — dado temporário
├── journeymap/, TCNodeTracker/,   ← dados/caches locais gerados pelos respectivos mods
│   compendiumunlocks/,              durante o jogo — não precisam ser versionados
│   compendiumUpdates/, local/,
│   mod-config/, data/
│
├── natives/                       ← DLLs nativas do LWJGL/Java (específicas do Windows)
├── falsepattern/                  ← dependências .jar baixadas automaticamente pelo FalsePatternLib
│
└── server-resource-packs/, modpack/, .gitignore, usernamecache.json, estrutura.txt
    (arquivos auxiliares / específicos do ambiente de quem mantém o pack)
```

> ⚠️ **Nota sobre o que é "o modpack" e o que é "dado de jogo pessoal":** as pastas `saves/`,
> `backups/`, `crash-reports/`, `logs/`, `journeymap/`, `TCNodeTracker/` e o arquivo
> `usernamecache.json` guardam progresso, mundo e cache **do ambiente de quem mantém o repositório**
> — não fazem parte do modpack em si e já estão listadas no `.gitignore` da raiz, então não sobem
> mais para o repositório remoto. Se for redistribuir só o pack (sem o mundo/progresso do
> mantenedor), copie apenas `mods/`, `config/`, `resourcepacks/`, `resources/`, `scripts/`,
> `ambience_music/`, `fonts/`, `options.txt` e os arquivos de versão (`Hogwarts.jar`/`.json`).

## Como instalar

### Opção 1 — TLauncher (recomendado, é o formato original deste pack)
O `TLauncherAdditional.json` na raiz indica que o pack foi feito e testado no TLauncher usando a
opção **"diretório de jogo separado"** por perfil. Para reproduzir exatamente esse ambiente:

1. Instale o [TLauncher](https://tlauncher.org/) e abra-o pelo menos uma vez para gerar a pasta
   `.minecraft` padrão.
2. Baixe/clone este repositório inteiro.
3. Copie a pasta inteira do repositório para dentro de `.minecraft/versions/`, renomeando-a para
   **`Hogwarts`** — o caminho final deve ficar `.minecraft/versions/Hogwarts/` contendo
   `Hogwarts.jar`, `Hogwarts.json`, `mods/`, `config/` etc. todos no mesmo nível.
4. Abra o TLauncher, vá em **Versões** → selecione **Hogwarts** (ela aparecerá automaticamente por
   causa do `Hogwarts.json`).
5. Nas configurações desse perfil, confirme que **"Diretório de jogo separado"** está marcado
   apontando para essa mesma pasta `Hogwarts/` — assim `mods/`, `saves/`, `config/` e `options.txt`
   serão lidos dali em vez da `.minecraft` raiz.
6. Aumente a RAM alocada para pelo menos 6 GB nas configurações do Java do perfil.
7. Salve, aponte pro IP do servidor (será divulgado no grupo quando estiver no ar) e bom jogo!

### Opção 2 — MultiMC / Prism Launcher
1. Crie uma instância nova: **Minecraft 1.7.10** + **Forge 10.13.4.1614**.
2. Clique em **Pasta de instância** (ou "Edit Instance" → "Open .minecraft") para abrir a pasta
   `.minecraft` interna dessa instância.
3. Copie o conteúdo deste repositório para dentro dessa pasta `.minecraft`, substituindo o que já
   existir (a subpasta `mods/` do launcher, se ela já tiver sido criada vazia, por exemplo).
4. Nas configurações da instância, aumente a memória (Java) para pelo menos 6 GB.
5. Copie também o `options.txt` para dentro dessa mesma pasta — ele já vem com os conflitos de
   tecla resolvidos e o HUD organizado (veja `KEYBINDS.md`). Se preferir manter suas próprias
   configurações de vídeo/som, copie só as linhas `key_*` dele.
6. Abra o jogo, aponte pro IP do servidor e bom jogo!

### Opção 3 — CurseForge App
O CurseForge app não lê a estrutura deste repositório diretamente (ele espera um pacote no formato
de modpack do CurseForge/Overwolf, com `manifest.json`). Para usar por ele:
1. Crie um perfil personalizado em branco para **Minecraft 1.7.10** com **Forge 10.13.4.1614**
   (no CurseForge app: **Criar Perfil Personalizado** → escolha a versão e o Forge certos).
2. Clique nos três pontinhos do perfil → **Abrir pasta** para achar a pasta local dele.
3. Copie o conteúdo deste repositório para dentro dessa pasta, do mesmo jeito descrito na Opção 2.
4. Ajuste a RAM alocada nas configurações do perfil (mínimo 6 GB) e bom jogo!

### Lançador "manual" / vanilla (sem launcher de terceiros)
Também é possível instalar Forge 1.7.10-10.13.4.1614 manualmente e copiar o conteúdo deste
repositório direto para dentro de `.minecraft` (a pasta padrão do launcher oficial da Mojang) —
o processo é o mesmo da Opção 2, só que usando o `.minecraft` do launcher oficial em vez do de um
launcher alternativo.

## Testando localmente antes do servidor
Este repositório está pronto pra qualquer um baixar e testar em **mundo local (singleplayer)**
antes do servidor oficial subir — é só seguir os passos de instalação acima e criar um mundo novo
pra experimentar os mods (sem precisar copiar a pasta `saves/` deste repositório).

## O que já foi ajustado nesse pack
- **HUD reorganizado**: vários mods de interface (Better HUD, WAILA, JourneyMap, Damage Indicators)
  brigavam pelo mesmo canto de tela. Foram redistribuídos pra não sobrepor.
- **Otimização de performance**: prioridade de tick por dimensão (`tickDynamic`), redução de
  entidade fora de alcance (`archaicfix`), limite sensato de chunkloading (`forgeChunkLoading`),
  despawn de mob selvagem ativado (`MoCreatures`), culling de renderização reativado (`fastcraft`).
- **Conflitos de tecla resolvidos** — detalhes em [`KEYBINDS.md`](KEYBINDS.md).
- **Limpeza de configs órfãs** de mods que foram testados e removidos (AE2, Netherlicious).
- **Troca do ID Conflicts Viewer pelo Dynamic Surroundings** — ver aviso importante em
  [`MODLIST.md`](MODLIST.md#aviso-importante-para-quem-for-jogar).

## Problemas conhecidos / em investigação
> ⚠️ Preencher depois de confirmar: os crash reports que apareciam antes dos ajustes de performance
> pararam de acontecer, ou a pasta `crash-reports/` só foi limpa manualmente? Se alguém tiver um
> crash, por favor suba o arquivo de dentro de `crash-reports/` num canal do grupo antes de apagar.

## Contribuindo / reportando problemas
Encontrou bug, travamento ou sobreposição de HUD? Abra uma issue neste repositório com:
- print da tela (se for visual)
- o arquivo de dentro de `crash-reports/` (se for travamento) — como essa pasta está no
  `.gitignore`, ela não sobe sozinha pro repositório: anexe o arquivo manualmente na issue ou
  suba num canal do grupo
- o que você estava fazendo no momento

## Créditos
Modpack montado por Daniel Velluto Bento, inspirado na série "Escola de Bruxos"
(AuthenticGames, Malena, Nofaxu). Todos os mods pertencem aos seus respectivos autores originais.
