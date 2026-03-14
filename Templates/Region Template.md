---
name: "{{title}}"
type: region
aliases: []
climate:
government:
population:
tags: [location, region]
---

# {{title}}

## Описание
*Общее описание региона.*

## География
*Рельеф, климат, природные особенности.*

## Население
*Народы, расы, культура.*

## Политика
*Власть, фракции, конфликты.*

## Экономика
*Торговля, ресурсы, богатства.*

## Локации

```dataview
TABLE type, tags FROM "Locations"
WHERE contains(region, this.name)
```

## Персонажи региона

```dataview
TABLE faction, status FROM "Characters"
WHERE region = this.name
```

---
*Связанные заметки:*
