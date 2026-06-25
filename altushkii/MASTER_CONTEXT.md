# MASTER CONTEXT — ПРОЕКТ АЛЬТУШКА + БЛОНДИНКА

Последнее обновление: 2026-06-25

---

## 1. ОБЗОР ПРОЕКТА

Два AI-персонажа для соцсетей (Instagram, TikTok, Telegram).
Цель — генерация фото/видео контента, рост аудитории, монетизация.

---

## 2. ПЕРСОНАЖ: АЛЬТУШКА

### Базовая идентичность

- Возраст: ранние 20 лет
- Кожа: очень бледная фарфоровая, холодный подтон, почти paper-white
- Волосы: messy jet-black choppy bob до подбородка, blunt straight bangs выше бровей, чёлка разделена на chunky секции с зазорами, текстура roughened, straw-like на кончиках
- Лицо: slim elongated oval, очень узкая челюсть, острый подбородок, высокие скулы с мягкими впадинами
- Глаза: узкие миндалевидные, серо-зелёные с olive undertone, slightly hooded, wide-set
- Подводка: thin precise winged black eyeliner, slightly imperfect, not symmetrical between eyes
- Губы: драматически увеличенные, filler aesthetic, nude-pink, matte-to-satin finish, доминантная черта лица
- Нос: тонкий, прямой, маленький
- Ногти: extremely long sharp stiletto acrylic, solid glossy pure black
- Выражение по умолчанию: calm, melancholic, emotionally restrained

### Trigger word LoRA: `altushka_v1`

### LoRA статус
- Обучена на FLUX.1-dev, rank 32, 2000 steps, lr 1e-4
- Файл: altushka_v1.safetensors (328MB)
- Загружена на CivitAI
- Обучена на RTX A6000 на RunPod (~$1.25)
- Датасет: 20 фото с кэпшнами

### Зафиксированные пресеты

**Altushka_phone:**
iPhone 16 Pro Natural Titanium (серый титан). Постоянное устройство во всех кадрах.
Опционально — прозрачный MagSafe чехол.

**Altushka_apartment_v1:**
Modern moody dark masculine apartment. Контрастные стены (тёмно-серая + бежевая). Тёмный паркет венге. OLED TV на стене. Кожаная кушетка под TV. Оливково-зелёное кресло. Большое напольное зеркало. Только тёплый янтарный свет 2700-3000K. Померанский шпиц рыже-оранжевый. Блэкаут-шторы. Вечерняя атмосфера всегда.

EN version для промптов:
```
Modern moody dark masculine apartment interior, evening atmosphere.
Contrasting walls — one wall dark grey matte with vertical decorative
panels, another wall beige-cream. Dark walnut hardwood floors.
Large flat-screen TV on dark wall, screen off. Low dark brown vintage
leather chaise lounge with quilted texture below TV. Accent olive-green
chair with thin black metal legs. Large dark-framed floor mirror.
Warm amber low-light only, no overhead white lighting, blackout curtains.
Optional small fluffy orange Pomeranian dog.
```

**Altushka_hands:**
```
Extremely thin bony feminine hands with disproportionately long slender
fingers, prominent visible knuckles and finger joints, pronounced tendons
on the back of the hand, very flat and narrow palm with almost no soft
tissue padding. Wrist extremely narrow and angular with visible ulna bone.
Skin porcelain-pale, smooth and clean. No rings, no bracelets, no jewelry.
Extremely long sharp stiletto acrylic nails, solid glossy pure black.
Exactly five fingers per hand.
```

**Altushka_evening_taxi:**
Короткое чёрное платье, белый кожаный салон, Тверская ночью, нога на ногу.

### Обновлённый промпт лица v2 (актуальный)
```
A specific young woman in her early twenties, extremely pale porcelain
skin with cool undertones, almost paper-white, natural skin texture
with visible fine pores.

Hair: messy jet-black choppy bob reaching jawline to chin length,
heavily textured with choppy razored layers, blunt straight bangs
cut precisely just above the eyebrows, bangs slightly uneven and
separated into chunky sections with small gaps showing the forehead.
Hair slightly dishevelled with natural flyaways. Texture straight
but roughened, almost straw-like at the ends. Hair frames the face
tightly on both sides, curving slightly inward at the jawline.

Face: slim elongated oval face, noticeably longer than wide. Extremely
narrow tapering jawline ending in a small sharp pointed chin.
Moderately prominent high cheekbones creating subtle natural hollows.

Eyes: narrow almond-shaped, horizontally elongated and slightly
wide-set. Soft desaturated grey-green iris with subtle olive undertone.
Slightly hooded upper eyelids. Calm, slightly melancholic gaze.
Thin precise winged black eyeliner on upper lash line only, slightly
imperfect, not perfectly symmetrical. Natural dark lashes. Eyebrows
natural, dark, slightly thin, low soft arch.

Nose: very thin straight small nose, narrow bridge, small refined tip.

Lips: dramatically oversized heavily volumized lips, strikingly
disproportionate to the rest of the face. Both upper and lower lip
extremely full and plump, lower lip slightly larger. Strong defined
cupid's bow. Natural nude-pink color with soft matte-to-satin finish.
The lips are by far the most dominant feature of the entire face.
```

---

## 3. ПЕРСОНАЖ: БЛОНДИНКА

### Базовая идентичность

- Возраст: 20-21 год
- Кожа: светлая, ровная, здоровое сияние, лёгкий загар
- Волосы: длинные, НЕЙТРАЛЬНЫЙ ХОЛОДНОВАТЫЙ СВЕТЛЫЙ БЛОНД (НЕ золотой, НЕ медовый, НЕ рыжеватый), лёгкая волна, центральный пробор
- Глаза: миндалевидные, янтарно-карие, опущенные внешние уголки
- Губы: огромные, filler aesthetic, snake bites (два серебристых пирсинга)
- Ногти: длинные миндалевидные, нюдовый глянец
- Украшения: тонкая золотая цепочка
- БЕЗ ТАТУИРОВОК (полностью чистая кожа)

### Trigger word LoRA: `blonda_v1`
### LoRA статус: тренировка начата, не завершена

### Ключевые уроки по промптингу
- `golden-blonde / sun-bleached / warm / luminous` → уводит в рыжину
- Правильно: `light blonde, neutral cool-toned, ash-blonde`
- Для ChatGPT Images: негативы переписывать в позитив
- Упоминание татуировок удалено из всех промптов

---

## 4. ТЕХНИЧЕСКИЙ СТЕК

### Генерация изображений
- **Nano Banana Pro** — основной генератор (подписка заканчивается через ~4 дня)
- **ChatGPT Images** — альтернатива для блондинки
- **Face swap** — отдельный второй шаг после генерации сцены

### Генерация видео
- **WanAnimate 2.2** через ComfyUI на RunPod
- Проблема: потеря консистентности лица на длинных видео
- Решение: снизить количество LoRA (оставить 2 из 5), поднять steps с 4 до 6-8, ratio в ClipVision с 0.5 до 0.75

### LoRA тренировка
- AI Toolkit на RunPod (RTX A6000)
- FLUX.1-dev base model

### Хостинг моделей
- CivitAI, HuggingFace

---

## 5. РАБОЧИЙ ПРОЦЕСС ГЕНЕРАЦИИ

### Фото (двухшаговый метод — обход фильтров):
1. Генерируем сцену из текстового промпта БЕЗ детального описания лица/тела
2. Face swap с референсом лица персонажа

### Face swap промпт (шаблон):
```
Replace the face of the woman in image 1 with the face from image 2.
Keep everything else from image 1 exactly unchanged: [перечислить позу,
одежду, фон, освещение]. The new face must seamlessly match the lighting
direction, skin tone, and shadow placement of the original scene.
Blend the face naturally into the neck and hairline. The hair must be
[описание волос] from image 2. The lips must be dramatically oversized
with obvious filler aesthetic from image 2. The result should look like
one real photograph of one real person, not a collage or edit.
Photorealistic, natural, no artifacts, no visible seams, no distortion.
```

### Обход фильтров Nano Banana — что триггерит:
- `semi-sheer`, `see-through`, `transparent` + одежда
- `crop top` + `low-rise` + описание фигуры в одном промпте
- `S-curve`, `arched lower back`, `contrapposto` + одежда
- `sculpting leggings`, `heart-shaped contour on glutes`
- Детальное описание губ + тела + позы всё вместе
- Фото реальных моделей/знаменитостей как референс

### Что работает:
- Генерить сцену отдельно, face swap отдельно
- Короткие промпты без детального описания тела
- `fitted` вместо `tight`, `top` вместо `crop top`
- `lace bottoms` вместо `bikini-cut panties`
- Убирать `midriff exposed`, `navel visible`

---

## 6. INSTAGRAM — ПЛАН ПРОГРЕВА

### Текущий статус
- Аккаунт зарегистрирован на немецких прокси и VPN
- День 1-2 прогрева (просто смотрел ленту)

### Фазы:
- **Дни 1-7:** минимальная активность, смотреть alt/goth тематику, 2-3 лайка в день
- **Дни 8-14:** нейтральные сторис и рилсы БЕЗ AI-контента (мемы, переписки). POV-фото без лица (ноги, руки, детали)
- **День 14:** проверить «Похожие авторы» в профессиональной панели
- **День 15+:** основной контент с лицом персонажа

### Правила:
- Первые 14 дней — никакого AI на аватарку
- Метаданные подставлять под геолокацию (ExifTool)
- 1 аккаунт = 1 прокси
- Никаких внешних ссылок первые 14 дней
- Bridge page вместо прямых ссылок на платформу монетизации

### Контент-план:
- 1 пост в день
- 2-3 рилса в неделю
- Первые фото — без лица, возможно не AI

---

## 7. ЦЕЛЕВАЯ АУДИТОРИЯ

- СНГ + англоязычная (параллельно)
- Формат: lifestyle + тренды (танцы позже, когда дотянем реализм)
- Воронка: Instagram → Telegram → монетизация

---

## 8. ЧТО НУЖНО СДЕЛАТЬ

- [ ] Паспорт альтушки (имя, характер, легенда, табу)
- [ ] Пачка POV-промптов без лица (неделя 2)
- [ ] Московские локации + промпты (неделя 3)
- [ ] Промпты для квартиры (selfie/mirror)
- [ ] Нагенерить ~30 фото + 3-5 видео за 4 дня
- [ ] Завершить LoRA блондинки
- [ ] Стабилизировать WanAnimate (убрать лишние LoRA)
- [ ] Создать Telegram-канал
- [ ] Паспорт блондинки
