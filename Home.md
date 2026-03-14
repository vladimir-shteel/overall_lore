# Добро пожаловать в Wiki сеттинга

## Быстрая навигация
- [[Characters/|Персонажи]]
- [[Locations/|Локации]]
- [[Events/|События]]
- [[Items/|Предметы]]
- [[Timeline/|Таймлайн]]

---

## Персонажи

```dataview
TABLE faction, region, status FROM "Characters"
SORT name ASC
```

---

## Последние события

```dataview
TABLE date, location FROM "Events"
SORT date DESC
LIMIT 10
```

---

## Локации

```dataview
TABLE location_type, region FROM "Locations"
SORT name ASC
```

---

## Предметы

```dataview
TABLE item_type, rarity, owner FROM "Items"
SORT name ASC
```

---

## Статистика

```dataview
TABLE length(rows) AS "Количество"
FROM ""
WHERE type
GROUP BY type
```
