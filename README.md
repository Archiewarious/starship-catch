# Поймай корабль

Browser game: land the Starship upper stage into the arms of the launch tower, the way it happened on Flight 15. One HTML file, no dependencies. The game text is in Russian.

**Играть:** https://archiewarious.github.io/starship-catch/

14 ноября 2026 года на Flight 15 корабль Starship впервые вернулся с орбиты и был пойман руками башни. В игре нужно повторить последние полторы минуты этого полёта. Корабль падает плашмя с 1500 м, ты наводишь его на башню, переворачиваешь, гасишь скорость и зависаешь между руками.

## Управление

| Клавиша | Что делает |
|---|---|
| A / D | плашмя рулить закрылками, после поджига сдвигаться вбок |
| Пробел | переворот и поджиг трёх двигателей |
| W / S | газ больше или меньше (от 40 до 100%) |
| Q / E | погасить или зажечь один двигатель |
| 1 / 2 / 3 | оставить столько двигателей |
| R | начать заново |

Стрелки тоже работают. На телефоне внизу экрана есть кнопки.

## Как сажать

1. Пока падаешь, своди жёлтый крестик на мини-карте с красным крестиком башни.
2. Когда высота у корабля станет жёлтой, жми пробел.
3. Через 4 секунды погаси один двигатель (Q), а когда падение замедлится до 10 м/с, погаси ещё один.
4. На одном двигателе спускайся газом и короткими нажатиями A/D держись над центром.
5. У рук почти зависни. Руки сомкнутся сами.

Ниже 40% тяги Raptor не работает, поэтому лишние двигатели гасят. Так же было на Flight 15: три двигателя, потом два, потом один.

## Режимы

**Обычный.** Двойной запас топлива, руки ловят корабль при промахе до 6,5 м, вбок управлять проще.

**Реализм.** Честные числа: промах до 2 м, касание не быстрее 2 м/с, наклон до 5°.

## Физика

Корабль 52 × 9 м и около 130 т на поджиге. Три двигателя по 250 тс, сопротивление воздуха зависит от высоты, ветер с порывами. SpaceX публикует не всё, поэтому массу, коэффициенты сопротивления и допуски поимки пришлось восстановить расчётом по наблюдаемым скоростям и таймингу Flight 15. Все числа собраны в объекте `CFG` в начале скрипта, у каждого помечено, откуда оно.

Источники:

- [Starship flight 15](https://en.wikipedia.org/wiki/Starship_flight_15), Wikipedia
- [SpaceX Raptor](https://en.wikipedia.org/wiki/SpaceX_Raptor), Wikipedia
- [SpaceX Starship (spacecraft)](https://en.wikipedia.org/wiki/SpaceX_Starship_(spacecraft)), Wikipedia
- [Starship's belly flop maneuver](https://everydayastronaut.com/starships-belly-flop-maneuver/), Everyday Astronaut
- [Starship Flight 15 ends with first ship tower catch](https://aviationweek.com/space/operations-safety/starship-flight-15-ends-first-ship-tower-catch), Aviation Week
- [Can SpaceX land a rocket with 1-2 cm accuracy?](https://theshamblog.com/can-spacex-land-a-rocket-with-1-2-cm-accuracy/), The Shamblog

## Запуск у себя

Скачай `index.html` и открой в браузере. Сервер не нужен.

Фанатский проект, со SpaceX никак не связан.

## Лицензия

[MIT](LICENSE)
