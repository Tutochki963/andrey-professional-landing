# VISUAL QA v0.2.1 — Andrey Professional Landing

**Статус:** browser review after warmer P0 redesign  
**Вердикт:** палитра и архитектура стали заметно лучше, но страница всё ещё местами выглядит как технический интерфейс. Следующая итерация должна смягчить типографику, добавить глубину и сделать интерактивность более дорогой и спокойной.

## Что стало лучше

- Ушла большая часть кислотного cyan / mint ощущения.
- Sand + blue-grey + sage психологически воспринимаются спокойнее.
- Hero стал лучше сбалансирован по масштабу.
- Working Path читается как система, а не декоративный объект.
- Track Record теперь имеет разные типы proof для разных периодов.
- Selected Work получил evidence slots вместо watermark.
- AI-STUDIO system map стал действительно архитектурой с зонами.
- Contact уже выглядит как следующий шаг, а не пустой footer.

## Главные проблемы текущей версии

### 1. Заголовки слишком тяжёлые

Основные h1 / h2 всё ещё набраны слишком жирно и крупно. Из-за этого страница визуально «кричит» и напоминает технологический лендинг стартапа больше, чем премиальное портфолио консультанта.

Нужно:
- снизить font-weight;
- уменьшить максимальный размер;
- увеличить line-height на 2–4%;
- сделать tracking менее агрессивным;
- использовать системный display stack: `Aptos Display / Segoe UI Variable Display / Segoe UI`.

### 2. Палитру нужно ещё смягчить

Текущий фон по-прежнему почти чёрный и местами ощущается сурово.

Нужно:
- слегка поднять светлоту базового графита;
- сделать основной текст чуть теплее;
- снизить контраст вторичного текста;
- accent-цвета сделать ещё менее насыщенными;
- убрать любые ощущения «security console».

### 3. Объём недостаточно выражен

Секции всё ещё живут преимущественно на одной плоскости.

Нужно создавать depth через:
- мягкие surface gradients;
- внутренний highlight верхней грани;
- спокойную elevation shadow;
- разные уровни panel brightness;
- локальные radial light fields.

Без glow и neon.

### 4. Hero balance

Сейчас hero уже рабочий, но можно улучшить:
- headline сделать чуть меньше и легче;
- system card сделать визуально глубже;
- связующую horizontal line сделать тоньше и мягче;
- Result выделять не яркостью, а тёплой поверхностью и depth.

### 5. Ритм секций

Случайных пустот стало меньше, но ещё заметны слишком большие паузы:
- после Track Record;
- перед Selected Work;
- после AI-STUDIO.

Нужно индивидуально уменьшить section padding, а не применять одинаковый rhythm.

### 6. Evidence slots

Структурно они теперь правильные, но пустые прямоугольники выглядят как wireframe.

До появления реальных public-safe assets:
- сделать placeholders более смысловыми;
- использовать schematic lines / nodes вместо пустых boxes;
- добавить маленький label типа `system map / workflow fragment / test-kit fragment`.

### 7. AI-STUDIO architecture

Архитектура уже читается хорошо.

Следующая задача — убрать ощущение dashboard:
- смягчить границы;
- сделать зоны визуально разной глубины, а не одинаковыми ячейками;
- rails ослабить;
- Human decision оставить самым явным control point.

### 8. Contact

Смысловая архитектура стала лучше.

Нужно:
- hover / focus states на реальных кнопках;
- плавная подсветка border + soft shadow;
- primary CTA должен давать тёплый feedback;
- pending channels не должны выглядеть кликабельными.

### 9. Где ещё остаётся «технический интерфейс»

- uppercase labels слишком частые;
- много прямых границ;
- одинаковая геометрия system panels;
- сильный контраст белого заголовка на почти чёрном фоне;
- строгая сетка без мягких визуальных переходов.

## Приоритет v0.2.2

P0:
1. Typography softening.
2. Softer graphite / warm-neutral palette.
3. Button hover / focus glow without neon.
4. More depth in hero, case cards and system map.
5. Reduce section gaps.

P1:
6. Improve evidence placeholders.
7. Soften AI-STUDIO grid geometry.
8. Reduce uppercase labels.

P2:
9. Mobile QA.
10. RU visual QA.
11. Motion only after composition is stable.
