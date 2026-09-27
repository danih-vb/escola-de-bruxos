# Escola de Bruxos — Lista de Mods

Modpack para **Minecraft 1.7.10** com **Forge 10.13.4.1614** • Criado por Daniel Velluto Bento
Lista extraída diretamente da pasta `mods/` e conferida contra o `fml-client-latest.log` mais
recente — **186 mods carregados pelo Forge**, distribuídos em **160 arquivos** `.jar`/`.zip`
(alguns arquivos, como o `ProjectRed`, o `WR-CBE` e o `NEI Addons`, empacotam mais de um mod dentro
do mesmo `.jar`, o que explica a diferença entre os dois números).

## Sobre o modpack
Escola de Bruxos é um modpack "kitchen sink" para Minecraft 1.7.10, construído e testado mod por mod,
em fases controladas, para rodar de forma estável num servidor privado entre amigos. O foco central é
a magia: o pack reúne vários sistemas mágicos completos e distintos rodando lado a lado — Thaumcraft
(com os addons Thaumic Tinkerer, Thaumic Exploration, ThaumicHorizons, Forbidden Magic e Automagy),
Witchery, Botania, Blood Magic (com o addon Sanguimancy), Ars Magica 2, AbyssalCraft e Cyano's Wonderful
Wands — cada um com sua própria progressão, permitindo que cada jogador escolha (ou combine) a escola de
magia que mais combina com seu estilo de jogo.

Além da magia, o pack cobre exploração (Twilight Forest, Biomes O' Plenty com o addon BiblioWoods,
Mystcraft, Roguelike Dungeons, Netherite), tecnologia e automação (Tinker's Construct com Tinkers'
Mechworks, Forestry, Extra Utilities, Ender IO com Ender Storage e Ender Tanks, ProjectRed, ProjectE,
RFTools, JABBA, MrTJPCore/ChickenChunks, FTB Utilities), uma boa variedade de mobs e criaturas (Mo'
Creatures, OreSpawn, Grimoire of Gaia, Mowzie's Mobs, Infernal Mobs, Exotic Birds, Necromancy), decoração
e armazenamento (Chisel, BiblioCraft, Carpenter's Blocks, Malisis' Doors, Storage Drawers, Iron Chest) e
um sistema de comida mais completo (Pam's HarvestCraft, Cooking for Blockheads, Master Chef, com fome
ajustada pelo Hunger Overhaul e cultivo sazonal via Serene Seasons). Também conta com progressão de
missões (BetterQuesting) e um End mais desafiador (Hardcore Ender Expansion).

## O que mudou desde a última lista
| Mod | Mod ID | Versão | Situação |
|---|---|---|---|
| BetterQuesting | betterquesting | 3.0.328 | ✅ Novo |
| bettersearch | bettersearch | 1.4.3 | ✅ Novo |
| Hardcore Ender Expansion | hardcoreenderexpansion | 1.8.6 | ✅ Novo |
| Dynamic Surroundings | dsurround | 1.0.6.4 | ✅ Novo (substitui o ID Conflicts Viewer) |
| ID Conflicts Viewer | idcv | 1.3 | ❌ Removido |

Nenhum outro mod da lista anterior (181 mods) foi alterado — todos continuam presentes e ativos.

## Aviso importante para quem for jogar
O **ID Conflicts Viewer** foi removido depois de confirmado que não haveria mais adição de mods.
Se no futuro alguém adicionar um mod extra por conta própria e ele conflitar com um ID já em uso
(bloco, item, bioma ou poção), **não existe mais a proteção automática de recusa de abertura** —
o problema só vai aparecer como corrupção de mundo ou crash. Portanto: **não adicione mods novos
sem consultar o grupo primeiro**, e sempre confira o `fml-client-latest.log` depois de qualquer mudança.

## Como essa lista foi montada
Esta lista foi gerada a partir do conteúdo real da pasta `mods/` (incluindo a subpasta `mods/1.7.10/`,
usada por alguns mods mais antigos). Ela cobre os **160 arquivos** de mod presentes, agrupados por
categoria para facilitar a leitura. Não incluímos aqui uma coluna de "Mod ID" individual para os 186
mods porque vários desses IDs só existem dentro do `.jar` (no `mcmod.info`) e não podem ser lidos com
segurança sem abrir cada arquivo — o `fml-client-latest.log` continua sendo a fonte 100% confiável e
atualizada automaticamente para conferir o Mod ID exato de qualquer mod (procure por
`Sending event FMLPreInitializationEvent to mod` para ver a lista dos 186 IDs, na ordem de carregamento).

## Lista completa de mods, por categoria

### Magia (19)

| Mod | Arquivo |
|---|---|
| AbyssalCraft | `AbyssalCraft-1.7.10-1.9.1.3-FINAL.jar` |
| Ars Magica 2 | `1.7.10_AM2-1.4.0.009.jar` |
| Automagy | `Automagy-1.7.10-0.28.2.jar` |
| Blood Magic | `BloodMagic-1.7.10-1.3.3-17.jar` |
| Botania | `Botania r1.8-249.jar` |
| Cyano's Wonderful Wands | `CyanosWonderfulWands-1.4.2.jar` |
| Forbidden Magic (addon Thaumcraft) | `Forbidden Magic-1.7.10-0.575.jar` |
| Magia Naturalis | `MagiaNaturalis-0.5.0.jar` |
| ProjectE | `ProjectE-1.7.10-PE1.10.1.jar` |
| Sanguimancy (addon Blood Magic) | `Sanguimancy-1.7.10-1.1.9-35.jar` |
| Sanguimancy Patch | `SanguimancyPatch-1.1.0.jar` |
| TC Helper (addon Thaumcraft) | `tchelper-1.7.10-1.4.jar` |
| TC Node Tracker (addon Thaumcraft) | `tcnodetracker-1.7.10-1.1.2.jar` |
| Thaumcraft | `Thaumcraft_1.7.10_4.2.3.5.jar` |
| Thaumcraft 4 Tweaks | `Thaumcraft4Tweaks-1.5.47.jar` |
| Thaumic Exploration (addon Thaumcraft) | `ThaumicExploration-1.7.10-1.1-53.jar` |
| Thaumic Tinkerer (addon Thaumcraft) | `ThaumicTinkerer-2.5-1.7.10-164.jar` |
| ThaumicHorizons (addon Thaumcraft) | `ThaumicHorizons-1.8.21.jar` |
| Witchery | `witchery-1.7.10-0.24.1.jar` |

### Exploração (8)

| Mod | Arquivo |
|---|---|
| BiblioWoods (addon Biomes O'Plenty) | `BiblioWoods[BiomesOPlenty][v1.9].jar` |
| Biomes O'Plenty | `BiomesOPlenty-1.7.10-2.1.0.2308-universal.jar` |
| Hardcore Ender Expansion | `HardcoreEnderExpansion  MC-1.7.10  v1.8.6.jar` |
| Mystcraft | `mystcraft-1.7.10-0.12.3.04.jar` |
| Natura | `natura-1.7.10-2.2.1a2.jar` |
| Netherite | `netherite-1.2+1.7.10.jar` |
| Roguelike Dungeons | `roguelike-1.7.10-1.5.0b.jar` |
| Twilight Forest | `TwilightForest-2.4.3.jar` |

### Tecnologia / Automação (19)

| Mod | Arquivo |
|---|---|
| ChickenChunks | `ChickenChunks-1.7.10-1.3.4.16-universal.jar` |
| Ender IO | `EnderIO-1.7.10-2.3.0.430_beta.jar` |
| Ender Storage | `EnderStorage-1.7.10-1.4.7.37-universal.jar` |
| Ender Tanks | `EnderTanks-rev16-beta1.jar` |
| Extra Utilities | `extrautilities-1.2.12.jar` |
| Extra Utilities Tweaks | `ExtraUtilitiesTweaks-1.0.0.jar` |
| Forestry | `forestry_1.7.10-4.2.16.64.jar` |
| FTB Utilities | `FTBUtilities-1.7.10-1.0.18.3.jar` |
| JABBA | `Jabba-1.2.2_1.7.10.jar` |
| Magical Crops | `magicalcrops-4.0.0_PUBLIC_BETA_3.jar` |
| ProjectRed - Base | `ProjectRed-1.7.10-4.7.0pre12.95-Base.jar` |
| ProjectRed - Integration | `ProjectRed-1.7.10-4.7.0pre12.95-Integration.jar` |
| ProjectRed - Lighting | `ProjectRed-1.7.10-4.7.0pre12.95-Lighting.jar` |
| ProjectRed - World | `ProjectRed-1.7.10-4.7.0pre12.95-World.jar` |
| RFTools | `rftools-4.23.jar` |
| TiC Tooltips (addon Tinkers' Construct) | `TiCTooltips-mc1.7.10-1.2.5.jar` |
| Tinkers' Construct | `TConstruct-1.7.10-1.8.8.build991.jar` |
| Tinkers' Mechworks | `TMechworks-1.7.10-0.2.15.106.jar` |
| WR-CBE (Wireless Redstone - CBE) | `WR-CBE-1.7.10-1.4.1.9-universal.jar` |

### Mobs / Criaturas (7)

| Mod | Arquivo |
|---|---|
| Exotic Birds | `Exotic Birds 1.7.10-1.4.6.jar` |
| Grimoire of Gaia 3 | `GrimoireOfGaia3-1.7.10-1.2.7.jar` |
| Infernal Mobs | `InfernalMobs-1.7.10.jar` |
| Mo' Creatures | `DrZharks MoCreatures Mod v6.3.1.zip` |
| Mowzie's Mobs | `MowziesMobs-1.2.99.jar` |
| Necromancy | `Necromancy-1.7.10.jar` |
| OreSpawn | `Ore-Spawn-Mod-1.7.10.jar` |

### Decoração / Armazenamento (10)

| Mod | Arquivo |
|---|---|
| Adventure Backpack | `adventurebackpack-1.7.10-0.8c.jar` |
| BiblioCraft | `BiblioCraft[v1.11.7][MC1.7.10].jar` |
| Carpenter's Blocks | `Carpenter's Blocks v3.3.8.2 - MC 1.7.10.jar` |
| Chisel | `Chisel-2.9.5.11.jar` |
| DecoCraft | `Decocraft-2.4.2_1.7.10.jar` |
| Iron Chest | `ironchest-1.7.10-6.0.39.728-universal.jar` |
| Malisis' Doors | `malisisdoors-1.7.10-1.13.2.jar` |
| MrCrayfish's Furniture Mod | `MrCrayfishFurnitureModv3.4.81.7.10.jar` |
| Storage Drawers | `StorageDrawers-1.7.10-1.10.9.jar` |
| Storage Drawers (addon Biomes O'Plenty) | `StorageDrawers-BiomesOPlenty-1.7.10-1.1.1.jar` |

### Comida (4)

| Mod | Arquivo |
|---|---|
| Cooking for Blockheads | `cookingbook-mc1.7.10-1.0.140.jar` |
| Hunger Overhaul | `HungerOverhaul-1.7.10-1.0.0.jenkins104.jar` |
| Master Chef | `MasterChef-1.7.10.jar` |
| Pam's HarvestCraft | `Pam's HarvestCraft 1.7.10Lb.jar` |
| Serene Seasons (estações do ano, afeta cultivo) | `SereneSeasons-1.7.10-1.2.18.jar` |

### Progressão / Missões (1)

| Mod | Arquivo |
|---|---|
| BetterQuesting | `BetterQuesting-3.0.328.jar` |

### Interface / HUD (25)

| Mod | Arquivo |
|---|---|
| Better Achievements | `BetterAchievements-1.7.10-0.1.0.jar` |
| Better HUD | `Better HUD by NukeDuck [1.7.10][1.3.5].jar` |
| BetterSearch | `bettersearch-forge-1.7.10-1.4.3.jar` |
| Command Keybindings | `Command Keybindings bp1.7.10(5.0.1.6).jar` |
| CraftingTweaks | `craftingtweaks-mc1.7.10-1.0.88.jar` |
| Custom Main Menu | `CustomMainMenu-MC1.7.10-1.9.2.jar` |
| Damage Indicators | `[1.7.10]DamageIndicatorsMod-3.3.2.jar` |
| Default Keys | `defaultkeys-mc1.7.10-1.0.28.jar` |
| Easy Config Button | `EasyConfigButton-1.0.jar` |
| Extra Achievements | `Extra Achievements 2.1.1.jar` |
| Inventory Control Keys | `InventoryControlKeys-1.7.10-1.0.1.jar` |
| Inventory Tweaks | `InventoryTweaks-1.59-dev-152.jar` |
| JourneyMap | `journeymap-forge-1.7.10-6.0.6.jar` |
| LLOverlay Reloaded | `LLOverlayReloaded-1.0.7-mc1.7.10.jar` |
| MystNEI Plugin (Mystcraft + NEI) | `MystNEI-Plugin-1.7.10-02.01.09.jar` |
| Neat | `Neat 1.0-1.jar` |
| NEI Addons | `neiaddons-1.12.15.41-mc1.7.10.jar` |
| NEI Integration | `NEIIntegration-MC1.7.10-1.1.2.jar` |
| Not Enough Items (NEI) | `NotEnoughItems-1.7.10-1.0.5.120-universal.jar` |
| Not Enough Keys | `NotEnoughKeys-1.7.10-3.0.0b45-dev-universal.jar` |
| Not Enough Resources | `NotEnoughResources-1.7.10-0.1.0-128.jar` |
| Thaumcraft NEI Plugin | `thaumcraftneiplugin-1.7.10-1.7a.jar` |
| Waila (What Am I Looking At) | `Waila-1.5.10_1.7.10.jar` |
| Waila Harvestability | `WailaHarvestability-mc1.7.10-1.1.6.jar` |
| Wawla (What Are We Looking At) | `Wawla-1.0.5.120.jar` |

### Visual / Gráficos (2)

| Mod | Arquivo |
|---|---|
| Better Foliage | `BetterFoliage-MC1.7.10-2.0.17.jar` |
| Blur | `Blur-MC1.7.10-1.0.1-2.jar` |

### Ambientação / Áudio (2)

| Mod | Arquivo |
|---|---|
| Ambience | `Ambience 1.0-3.jar` |
| Dynamic Surroundings | `DynamicSurroundings-1.7.10-1.0.6.4.jar` |

### Performance / Otimização (6)

| Mod | Arquivo |
|---|---|
| AI Improvements | `AIImprovements-1.7.10-0.0.1b8.jar` |
| ArchaicFix | `archaicfix-0.8.0.jar` |
| ChunkPurge | `ChunkPurge-1.7.10-2.1.jar` |
| FastCraft | `fastcraft-1.25.jar` |
| FoamFix | `FoamFix-1.7.10-universal-1.0.4.jar` |
| TickDynamic | `TickDynamic-1.7.10-0.1.5.jar` |

### Bibliotecas / APIs / Coremods (32)

| Mod | Arquivo |
|---|---|
| Animation API | `AnimationAPI-1.7.10-1.2.4.jar` |
| AppleCore | `AppleCore-mc1.7.10-3.1.1.jar` |
| Aroma1997Core | `Aroma1997Core-1.7.10-1.0.2.16.jar` |
| ASJCore | `1.7.10-ASJCore-1.7.0.1.jar` |
| Baubles | `Baubles-1.7.10-1.0.1.10.jar` |
| bdlib | `bdlib-1.9.5.1-mc1.7.10.jar` |
| bspkrsCore | `[1.7.10]bspkrsCore-universal-6.16.jar` |
| CodeChickenCore | `CodeChickenCore-1.7.10-1.0.7.48-universal.jar` |
| CodeChickenLib | `CodeChickenLib-1.1.10.jar` |
| CoFHLib | `CoFHLib-[1.7.10]1.2.1-185.jar` |
| EnderCore | `EnderCore-1.7.10-0.2.0.40_beta.jar` |
| FalsePatternLib | `falsepatternlib-mc1.7.10-1.12.2.jar` |
| Forge Multipart | `ForgeMultipart-1.7.10-1.2.0.345-universal.jar` |
| FTB Lib | `FTBLib-1.7.10-1.0.18.3.jar` |
| Gilded Games Util | `gilded-games-util-1.7.10-2.0.jar` |
| GTNHLib | `gtnhlib-0.11.51.jar` |
| Guide-API | `Guide-API-1.7.10-1.0.1-29.jar` |
| iChunUtil | `iChunUtil-4.2.3.jar` |
| LibSandstone | `LibSandstone-1.0.0.jar` |
| LLibrary | `llibrary-1.5.2-1.7.10.jar` |
| MalisisCore | `malisiscore-1.7.10-0.14.3.jar` |
| Mantle | `Mantle-1.7.10-0.3.2b.jar` |
| McJtyLib | `mcjtylib-1.8.1.jar` |
| MobiusCore | `MobiusCore-1.2.5_1.7.10.jar` |
| MrTJPCore | `MrTJPCore-1.7.10-1.1.0.33-universal.jar` |
| Not Enough IDs | `NotEnoughIDs-1.4.3.5.jar` |
| OpenModsLib | `OpenModsLib-1.7.10-0.10.1.jar` |
| Resource Loader | `ResourceLoader-MC1.7.10-1.3.jar` |
| SDNF | `sdnf-1.0.jar` |
| ShetiPhianCore | `ShetiPhianCore-1.7.10-3.0.0.jar` |
| SpACore | `SpACore-1.7.10-01.05.12.jar` |
| UniMixins | `%2Bunimixins-all-1.7.10-0.3.1.jar` |

### Utilidades diversas (24)

| Mod | Arquivo |
|---|---|
| AromaBackup | `AromaBackup-1.7.10-0.1.0.0.jar` |
| Balkon's WeaponMod | `weaponmod-1.14.3.jar` |
| BBG (Better Beacon Glow) | `BBG-1.0.0.jar` |
| CraftTweaker (MineTweaker 3) | `CraftTweaker-1.7.10-3.1.0-legacy.jar` |
| Ender Compass | `EnderCompass-1.7.10-1.2.jar` |
| Et Futurum | `etfuturum-2.6.2.jar` |
| Floocraft | `Floocraft-1.7.10-1.7.jar` |
| Fullscreen Windowed (Borderless) | `FullscreenWindowed-1.7.10-1.3.0b.jar` |
| Keeping Inventory | `KeepingInventory-1.7.10-2.1.jar` |
| Loot Bags | `LootBags-1.7.10-2.0.17.jar` |
| MineTweaker Recipe Maker | `MineTweakerRecipeMaker-1.7.10-1.1.1.jar` |
| Modpack Configuration Checker | `Modpack Configuration Checker-1.7.10-v1.5.3.jar` |
| Morph | `Morph-Beta-0.9.3.jar` |
| Nether Portal Fix | `netherportalfix-mc1.7.10-1.1.0.jar` |
| No Mob Spawning On Trees | `NoMobSpawningOnTrees-1.2.0-mc1.7.10.jar` |
| No More Recipe Conflict | `NoMoreRecipeConflict-0.3(1.7.10).jar` |
| OpenBlocks | `OpenBlocks-1.7.10-1.6.jar` |
| Rotten Flesh To Leather | `RottenFleshToLeather-2.1-1.7.10.jar` |
| Sleep | `Sleep-1.7.10-0.0-1.jar` |
| Step Up | `StepUp-1.0.1-mc1.7.10.jar` |
| Time In A Bottle | `time-in-a-bottle-1.7.10-1.0.2.jar` |
| TLSkinCape | `tlskincape1.7.10-1.4.jar` |
| Treecapitator | `1.7.10Treecapitator_universal_2.0.4.jar` |
| ZDoctorBB | `ZDoctorBB-1.7.10-Server.jar` |
