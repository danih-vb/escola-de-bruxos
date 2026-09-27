# Escola de Bruxos — Mapa de Atalhos Customizados

Com 186 mods instalados, várias teclas padrão colidiam (duas ou mais ações na mesma tecla).
Os conflitos reais (ações que disparam durante o jogo normal) foram remapeados. Conflitos que
ficam só dentro de uma tela específica de mod (CraftingTweaks, NotEnoughKeys, JourneyMap em tela
cheia) não foram mexidos — não causam problema real na prática.

Este documento tem duas partes:
1. **O que foi remapeado e por quê** (o histórico dos conflitos resolvidos).
2. **Referência completa de todos os atalhos** do modpack, mod por mod — incluindo os que nunca
   tiveram conflito e por isso continuam na tecla padrão de fábrica.

---

## Parte 1 — O que foi remapeado

### Teclas remapeadas

| Ação | Mod | Tecla nova | Tecla original |
|---|---|---|---|
| Atirar projétil | ProjectE | **Num7** | R |
| Modo da chave inglesa | Extra Utilities (Yeta Wrench) | **Num8** | Y |
| Cinto (HUD) | Tinkers' Construct / ttmisc | **Num9** | U |
| Óculos (HUD) | Tinkers' Construct / ttmisc | **Num5** | I |
| Alternar armadura | ttmisc | **Num6** | P |
| Alternar armadura | ProjectE | **Num.** | F |
| Atirar Lágrima de Sangue | Não identificado com certeza (ver Parte 2) | **Num*** | G |
| Nomes de entidades no minimapa | JourneyMap | **Num/** | G |
| Modo | ProjectE | **Num,** | G |
| Alternar estilo do minimapa | JourneyMap | **NumLock** | J |
| Localizador de som | Dynamic Surroundings (provável) | **ScrollLock** | L |
| Carregar | ProjectE | **CapsLock** | V |
| Customização de aura | Ars Magica 2 | **Pause** | V |
| Abrir missões | BetterQuesting | **Num Enter** | Y (colidia com foco do wand) |
| Abrir compêndio/guia | Guide-API | **Alt direito** | P (colidia com Visão Noturna) |

### Teclas desativadas (sem substituto — sem tecla física livre sobrando)
| Ação | Mod | Motivo |
|---|---|---|
| Função secundária do wand | Magia Naturalis | tecla F4 ficou só com o overlay de luz (mais usado) |
| Abrir tela de configuração | Better Foliage | tecla F8 ficou só com câmera suave (recurso do jogo); dá pra acessar essa config pelo menu de mods |

Se algum desses dois fizer falta, é só entrar em **Opções → Controles** no jogo e escolher uma
tecla livre — a essa altura sobra muito pouca tecla física de sobra, então talvez valha desativar
algo que você não usa antes de reatribuir.

### Por que numpad / teclas raras?
Depois de resolver os primeiros conflitos, restaram só 13 teclas realmente livres no teclado padrão
(numérico + CapsLock/ScrollLock/NumLock/Pause). Quando dois mods novos trouxeram mais 2 conflitos
reais, sobravam só **Num Enter** e **Alt direito** como opções — por isso essas duas entraram no jogo.

⚠️ **Se algum jogador usa notebook sem teclado numérico completo**, essas teclas podem não existir
fisicamente. Nesse caso, entre em Opções → Controles e reatribua manualmente para uma tecla de sua
preferência que esteja livre no seu teclado.

---

## Parte 2 — Referência completa de todos os atalhos

Esta lista cobre **todo** atalho configurável presente no `options.txt` do pack, extraído
diretamente do arquivo e convertido para nome de tecla legível — não só os que foram remapeados.
Ela está organizada por mod, na mesma ordem em que cada mod aparece na tela **Opções → Controles**
do jogo (que agrupa os atalhos pelo nome do mod que os registrou).

> 💡 Onde está escrito **"— (nenhuma tecla / desativada)"** ou **"— (desativada)"**, o atalho existe
> no mod mas não tem tecla nenhuma atribuída (o jogador precisa ir em Opções → Controles e escolher
> uma tecla manualmente se quiser usar aquela função).
>
> Onde está escrito **"provável"** ou **"Não identificado com certeza"**, não conseguimos confirmar
> com 100% de certeza a que mod aquele atalho pertence só a partir do `options.txt` — a forma mais
> confiável de confirmar é abrir **Opções → Controles** no jogo, que mostra o nome do mod acima de
> cada grupo de atalhos.

### Controles padrão do Minecraft (vanilla)

| Ação | Tecla atual |
|---|---|
| `key.attack` | **Botão esquerdo do mouse (Atacar)** |
| `key.use` | **Botão direito do mouse (Usar)** |
| `key.pickItem` | **Botão do meio do mouse (Pick Block)** |
| `key.forward` | **W** |
| `key.left` | **A** |
| `key.back` | **S** |
| `key.right` | **D** |
| `key.jump` | **Espaço** |
| `key.sneak` | **Shift esquerdo** |
| `key.sprint` | **Ctrl esquerdo** |
| `key.drop` | **Q** |
| `key.inventory` | **E** |
| `key.chat` | **T** |
| `key.command` | **/** |
| `key.playerlist` | **Tab** |
| `key.screenshot` | **F2** |
| `key.togglePerspective` | **F5** |
| `key.smoothCamera` | **F8** |
| `key.fullscreen` | **F11** |
| `key.hotbar.1` | **1** |
| `key.hotbar.2` | **2** |
| `key.hotbar.3` | **3** |
| `key.hotbar.4` | **4** |
| `key.hotbar.5` | **5** |
| `key.hotbar.6` | **6** |
| `key.hotbar.7` | **7** |
| `key.hotbar.8` | **8** |
| `key.hotbar.9` | **9** |

### Ars Magica 2

| Ação | Tecla atual |
|---|---|
| `key.ActivateAffinityAbility` | **F7** |
| `key.AuraCustomization` | **Pause** |
| `key.SpellBookNext` | **0** |
| `key.SpellBookPrev` | **M** |
| `key.ShapeGroups` | **F9** |
| `key.ToggleManaDisplay` | **]** |
| `Change Wand Focus` | **'** |
| `Change Arcane Lens` | **End** |
| `Activate Hover Harness` | **H** |
| `Glider Toggle` | **G** |
| `Misc Wand Toggle` | **`** |
| `Toggle Spider Climb` | **Delete** |
| `Toggle Chameleon Skin` | **Insert** |
| `Activate Morphic Fingers` | **Page Down** |

### Thaumcraft (+ addons)

| Ação | Tecla atual |
|---|---|
| `key.aspectMenu` | **I** |
| `Solve TC Research Node` | **Num+** |

### ProjectE

| Ação | Tecla atual |
|---|---|
| `pe.key.armor_toggle` | **Num.** |
| `pe.key.charge` | **CapsLock** |
| `pe.key.extra_function` | **C** |
| `pe.key.fire_projectile` | **Num7** |
| `pe.key.mode` | **Num,** |

### Extra Utilities (Yeta Wrench / Electromagnet)

| Ação | Tecla atual |
|---|---|
| `Yeta Wrench Mode` | **Num8** |
| `Toggle Electromagnet` | **— (nenhuma tecla / desativada)** |

### Tinkers' Construct / ttmisc (Travel Gear)

| Ação | Tecla atual |
|---|---|
| `key.tarmor` | **Y** |
| `key.tgoggles` | **Num5** |
| `key.tbelt` | **Num9** |
| `key.tzoom` | **Z** |
| `ttmisc.toggleArmor` | **Num6** |
| `Toggle StepUp` | **J** |

### JourneyMap

| Ação | Tecla atual |
|---|---|
| `key.journeymap.create_waypoint` | **B** |
| `key.journeymap.fullscreen.disable_buttons` | **— (desativada)** |
| `key.journeymap.fullscreen.east` | **Seta para direita** |
| `key.journeymap.fullscreen.north` | **Seta para cima** |
| `key.journeymap.fullscreen.south` | **Seta para baixo** |
| `key.journeymap.fullscreen.west` | **Seta para esquerda** |
| `key.journeymap.fullscreen_chat_position` | **C** |
| `key.journeymap.fullscreen_create_waypoint` | **B** |
| `key.journeymap.fullscreen_follow_player` | **F** |
| `key.journeymap.fullscreen_options` | **O** |
| `key.journeymap.fullscreen_waypoints` | **N** |
| `key.journeymap.map_toggle_alt` | **NumLock** |
| `key.journeymap.minimap_preset` | **\** |
| `key.journeymap.minimap_toggle_alt` | **— (desativada)** |
| `key.journeymap.minimap_type` | **[** |
| `key.journeymap.toggle_entity_names` | **Num/** |
| `key.journeymap.toggle_render_waypoints` | **— (desativada)** |
| `key.journeymap.toggle_render_waypoints_map` | **— (desativada)** |
| `key.journeymap.toggle_render_waypoints_world` | **— (desativada)** |
| `key.journeymap.toggle_waypoints` | **— (desativada)** |
| `key.journeymap.zoom_in` | **=** |
| `key.journeymap.zoom_out` | **-** |

### Waila

| Ação | Tecla atual |
|---|---|
| `waila.keybind.liquid` | **Num2** |
| `waila.keybind.recipe` | **Num3** |
| `waila.keybind.usage` | **Num4** |
| `waila.keybind.wailaconfig` | **Num0** |
| `waila.keybind.wailadisplay` | **Num1** |

### BetterQuesting

| Ação | Tecla atual |
|---|---|
| `key.betterquesting.quests` | **Num Enter** |

### BetterSearch

| Ação | Tecla atual |
|---|---|
| `key.bettersearch.open` | **O** |

### Better HUD

| Ação | Tecla atual |
|---|---|
| `key.betterHud.open` | **U** |

### Better Foliage

| Ação | Tecla atual |
|---|---|
| `key.betterfoliage.gui` | **— (nenhuma tecla / desativada)** |

### CraftingTweaks

| Ação | Tecla atual |
|---|---|
| `key.craftingtweaks.balance` | **B** |
| `key.craftingtweaks.clear` | **C** |
| `key.craftingtweaks.compress` | **K** |
| `key.craftingtweaks.decompress` | **— (nenhuma tecla / desativada)** |
| `key.craftingtweaks.rotate` | **R** |
| `key.craftingtweaks.toggleButtons` | **— (nenhuma tecla / desativada)** |

### Inventory Tweaks

| Ação | Tecla atual |
|---|---|
| `invtweaks.key.sort` | **R** |

### Adventure Backpack

| Ação | Tecla atual |
|---|---|
| `keys.adventureBackpack.openBackpackInventory` | **L** |
| `keys.adventureBackpack.switchHoseTank` | **K** |

### Baubles

| Ação | Tecla atual |
|---|---|
| `Baubles Inventory` | **;** |

### Magia Naturalis

| Ação | Tecla atual |
|---|---|
| `key.magianaturalis.decrease_size` | **Num-** |
| `key.magianaturalis.increase_size` | **Num+** |
| `key.magianaturalis.misc` | **— (nenhuma tecla / desativada)** |
| `key.magianaturalis.pick_block` | **Home** |

### Automagy

| Ação | Tecla atual |
|---|---|
| `Automagy.key.focusCrafting` | **F12** |

### ASJCore

| Ação | Tecla atual |
|---|---|
| `asjcore.orthoProjection` | **F6** |
| `asjcore.noEntityInteract` | **F10** |

### OpenBlocks (Vario / altímetro)

| Ação | Tecla atual |
|---|---|
| `openblocks.keybind.vario_switch` | **V** |
| `openblocks.keybind.vario_vol_down` | **— (nenhuma tecla / desativada)** |
| `openblocks.keybind.vario_vol_up` | **— (nenhuma tecla / desativada)** |

### LLOverlayReloaded

| Ação | Tecla atual |
|---|---|
| `key.llor.hotkey` | **F4** |

### Mo'Creatures

| Ação | Tecla atual |
|---|---|
| `MoCreatures Dive` | **F1** |
| `MoCreatures GUI` | **F3** |

### OreSpawn

| Ação | Tecla atual |
|---|---|
| `OreSpawn UP/FAST` | **Alt esquerdo** |

### Localizador de som (Dynamic Surroundings)

| Ação | Tecla atual |
|---|---|
| `Sound Locator` | **ScrollLock** |

### Witchery

| Ação | Tecla atual |
|---|---|
| `Night Vision` | **P** |
| `Goggles of Revealing` | **R** |

### Guia / Compêndio (Guide-API)

| Ação | Tecla atual |
|---|---|
| `key.openCompendium` | **Alt direito** |

### BiblioCraft (provável — navegação de fichário/quadro)

| Ação | Tecla atual |
|---|---|
| `key.columnshiftup` | **Y** |
| `key.columnshiftdown` | **H** |
| `key.columnbarup` | **U** |
| `key.columnbardown` | **J** |
| `key.portaitreposition` | **.** |

### Command Keybindings (atalhos de comando customizados)

| Ação | Tecla atual |
|---|---|
| `Command Key: /help` | **— (nenhuma tecla / desativada)** |
| `Command Key: /weather thunder` | **— (nenhuma tecla / desativada)** |

### Não identificado com certeza

| Ação | Tecla atual |
|---|---|
| `key.control` | **,** |
| `key.fart.desc` | **X** |
| `Step Assist` | **— (nenhuma tecla / desativada)** |
| `Speed` | **— (nenhuma tecla / desativada)** |
| `Jump` | **— (nenhuma tecla / desativada)** |
| `Shoot Normal Tear` | **F** |
| `Shoot Blood Tear` | **Num*** |


---

## Sobre mods citados que não aparecem aqui com atalho próprio

- **Witchery**: a maior parte das interações (rituais, poções, itens) é feita por uso direto de
  item/bloco, sem tecla dedicada. Os únicos dois atalhos identificados no `options.txt` que batem
  com itens de Witchery são **Visão Noturna** (`Night Vision`, tecla **P**) e **Óculos de
  Revelação** (`Goggles of Revealing`, tecla **R** — compartilhada com CraftingTweaks e Inventory
  Tweaks, mas sem conflito real porque cada um só age dentro do seu próprio contexto de tela).
- **Morph**: não encontramos nenhum atalho de teclado associado a esse mod no `options.txt` desta
  instalação. Isso normalmente significa que, nesta versão do Morph, a troca de forma é feita pela
  tela/GUI do mod em vez de um atalho de teclado dedicado — vale conferir dentro do jogo (tecla
  padrão do Morph, quando existe, costuma ser configurável em Opções → Controles, procurando pelo
  nome "Morph" no topo da lista).

## Como conferir/alterar qualquer atalho no jogo
1. Abra o jogo e vá em **Opções → Controles**.
2. Os atalhos aparecem agrupados pelo nome do mod (o mesmo agrupamento usado na Parte 2 deste
   documento).
3. Clique no atalho que quer mudar e pressione a nova tecla desejada. O jogo avisa na hora se a
   tecla escolhida já está em uso por outra ação **no mesmo contexto**.
