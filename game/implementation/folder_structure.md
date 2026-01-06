jrpg game

res://
│
├── scenes/
├── scripts/
├── assets/
├── data/
├── ui/
├── systems/
├── autoload/
└── debug/

scenes/
├── world/
│ ├── overworld.tscn
│ ├── town_01.tscn
│ ├── dungeon_01.tscn
│
├── battle/
│ ├── battle_scene.tscn
│ ├── enemy_group.tscn
│
├── characters/
│ ├── player.tscn
│ ├── npc.tscn
│
├── events/
│ ├── cutscene_dialogue.tscn
│
└── ui/
├── main_menu.tscn
├── pause_menu.tscn

scripts/
├── characters/
│ ├── player.gd
│ ├── npc.gd
│
├── battle/
│ ├── battle_manager.gd
│ ├── turn_queue.gd
│ ├── enemy_ai.gd
│
├── world/
│ ├── map_controller.gd
│ ├── encounter_manager.gd
│
├── events/
│ ├── dialogue_system.gd
│ ├── event_trigger.gd
│
└── utils/
├── math_helpers.gd

assets/
├── sprites/
│ ├── characters/
│ ├── enemies/
│ ├── tilesets/
│
├── audio/
│ ├── music/
│ ├── sfx/
│
└── fonts/

data/
├── characters/
│ ├── cecil.tres
│ ├── rosa.tres
│
├── enemies/
│ ├── goblin.tres
│ ├── dragon.tres
│
├── items/
│ ├── potion.tres
│ ├── ether.tres
│
├── skills/
│ ├── fire.tres
│ ├── cure.tres
│
└── jobs/
├── dark_knight.tres

ui/
├── hud/
│ ├── party_status.tscn
│
├── battle/
│ ├── command_menu.tscn
│ ├── target_selector.tscn
│
└── dialogue/
├── dialogue_box.tscn

systems/
├── save_system.gd
├── inventory_system.gd
├── audio_manager.gd

autoload/
├── game_state.gd
├── party_manager.gd
├── flags.gd

debug/
├── test_battle.tscn
├── enemy_spawner.gd

- architechtúra:
  WorldScene
  ↓ encounter
  BattleScene
  ↓ victory/defeat
  WorldScene
