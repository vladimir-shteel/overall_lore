---
name: "{{title}}"
type: location
aliases: []
region:
location_type: city
population:
tags: [location]
---

# {{title}}

## Описание
*Краткое описание места.*

## Атмосфера
*Как выглядит, запахи, звуки, ощущения.*

## История
*Как возникло, ключевые события.*

## Достопримечательности
*Важные места внутри локации.*

## Жители

```dataview
TABLE faction, status FROM "Characters"
WHERE location = this.name
```

## События здесь

```dataview
TABLE date, type FROM "Events"
WHERE contains(location, this.name)
SORT date ASC
```

---
*Связанные заметки:*
