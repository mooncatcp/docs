# Канал
Структура канала:
```json5
{
  id: "string", // Айди канала
  name: "string", // Название канала
  "group?": Group, // Группа, в которой находится канал. Если не указана - это личные сообщения
  type: 0, // Тип канала
  "position?": 0, // Позиция канала
  permission_overwrites: [PermissionOverwrite], // Массив правил измененных прав
  "topic?": "string", // Топик канала
  last_message_id: "string", // Айди последнего сообщения в канале
  "parent_id?": "string", // Айди категории (Если это канал в категории)
  "children?": [Channel], // Массив каналов в категории
}
```

## Типы каналов
| Тип | Описание         |
|-----|------------------|
| 0   | Текстовый канал  |
| 1   | Категория        |
| 2   | Личные сообщения |