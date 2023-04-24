# Права для пользователей или каналов
Доступность - где применимы права.<br>
Г - Группа (Глобально для всех каналов или права отвечающие за изменение группы), Л - Личные сообщения, К - Канал<br>
Все ограничения по правам, кроме личных сообщений, применяются только к ролям, т.е если у вас есть роль "Плохой человек" и канал "Для хороших людей", то вы просто убираете право читать сообщения в этом канале для этой роли.

| Значение |    Название     | Описание                                                                | Доступность |
|:--------:|:---------------:|:------------------------------------------------------------------------|:-----------:|
|  1 << 0  |  READ_MESSAGES  | Просмотр канала или сообщений в нём                                     |      К      |
|  1 << 1  | CREATE_MESSAGES | Отправка сообщений в канал                                              |      К      |
|  1 << 2  | MANAGE_MESSAGES | Управлять всеми сообщениями (Например удалять)                          |    Г, К     |
|  1 << 3  |  ADD_REACTIONS  | Добавлять реакции к сообщениям                                          |    Г, К     |
|  1 << 4  |  ATTACH_FILES   | Прикреплять аттачменты к сообщениям                                     |    Г, К     |
|  1 << 5  |  MANAGE_ROLES   | Управление ролями в группе (Добавление, удаление, изменение)            |      Г      |
|  1 << 6  |  MANAGE_USERS   | Управление пользователями (Изменение никнейма, ролей)                   |      Г      |
|  1 << 7  |   BAN_MEMBERS   | Банить людей в группе                                                   |      Г      |
|  1 << 8  |  KICK_MEMBERS   | Кикать людей с группы                                                   |      Г      |
|  1 << 9  |  MANAGE_GROUP   | Управление группой (Изменение названия/иконки, добавление эмодзи и т.д) |      Г      |
| 1 << 10  | MANAGE_CHANNELS | Управление каналами (Создание, перемещение и т.д)                       |      Г      |
| 1 << 11  |  ADMINISTRATOR  | Право администратора, дает все права.                                   |      Г      |