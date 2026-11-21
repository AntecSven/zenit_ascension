# Zenit Ascension - мод для приватного сервера Майнкрафт "Зенит"
> [!WARNING]
> **VIBECODE ATTENTION!** Весь код, кроме текстур и локализации сгенерирован нейросетью.

Требования:
Minecraft Java 26.3, Fabric Loader 0.20.1, Fabric API 0.166.2+26.3.
# Конфиг
Путь до конфигурационного файла: config/zenit_ascension/perks.json 
```
{
  "branches": [
    {
      "id": "mining",
      "title": "Добыча",
      "description": "Ветка развития добычи",
      "icon": "minecraft:iron_pickaxe",
      "background": "minecraft:textures/gui/advancements/backgrounds/stone.png",
      "effect": { "attribute": "block_break_speed", "percent": 5 },
      "cost": 0,
      "nodes": [
        {
          "id": "mining_i",
          "title": "Крепкая кирка",
          "description": "+10% к скорости разрушения блоков",
          "icon": "minecraft:stone_pickaxe",
          "x": 1, "y": 0,
          "parent": "mining",
          "effect": { "attribute": "block_break_speed", "percent": 10 }
        }
      ]
    }
  ]
}
```
`attribute` можно писать как `block_break_speed`, `minecraft:block_break_speed` или `player.block_break_speed`
