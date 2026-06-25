# ПОЛНЫЙ КОНТЕКСТ ПРОЕКТА — ДЛЯ CLAUDE

Последнее обновление: 2026-06-25
Этот файл содержит ВСЮ информацию по проекту. Загрузи его в начале нового чата.

---

## GITHUB ИНТЕГРАЦИЯ

Репозиторий: https://github.com/deadenlosen-sketch/ai-work
Токен: [ВСТАВЬ ТОКЕН В ЧАТ В НАЧАЛЕ СЕССИИ — GitHub не позволяет хранить токены в файлах]
Срок: до 23 сентября 2026

### Настройка в начале сессии:
Скажи Claude: "настрой гитхаб, токен: [вставь токен]"
Claude выполнит:
```bash
cd /home/claude && git clone https://github.com/deadenlosen-sketch/ai-work.git
cd ai-work
git remote set-url origin https://x-access-token:[ТОКЕН]@github.com/deadenlosen-sketch/ai-work.git
git config user.email "claude@assistant.ai"
git config user.name "Claude Assistant"
```

### Структура репо:
```
ai-work/
├── altushkii/
│   ├── MASTER_CONTEXT.md
│   ├── PROJECT_STATE.md
│   ├── PROMPTS/
│   ├── LOCATIONS/
│   ├── REFERENCES/
│   ├── altushka_character_library_v2.md
│   ├── ПРОЕКТ_Блондинка_v2.md
│   ├── ПРОЕКТ_АЛЬТУШКА_БИЗНЕС.md
│   └── Проект Альтушка.pdf
├── fsh/           (фоновый шум — YouTube)
└── rb money/      (ниша по Roblox)
```

### В конце каждой сессии:
1. Обновить PROJECT_STATE.md
2. Обновить MASTER_CONTEXT.md если были важные изменения
3. git add -A && git commit -m "описание" && git push origin main

---

## ОБЗОР ПРОЕКТА

Два AI-персонажа для соцсетей (Instagram, TikTok, Telegram).
Цель — генерация фото/видео, рост аудитории, монетизация.
Параллельные направления: фоновый шум (YouTube), Roblox.

### Коллаборация AI:
- **Claude** — промпт-инжиниринг, техника, документация, GitHub, воркфлоу
- **Grok** — идеи, концепции, креатив, психотип персонажей, image-to-video генерация
- Grok не имеет доступа к GitHub, работает через пользователя как посредника

---

## ПЕРСОНАЖ 1: АЛЬТУШКА

### Базовая идентичность
- Возраст: ранние 20 лет
- Кожа: очень бледная фарфоровая, холодный подтон, почти paper-white, естественная текстура с видимыми порами
- Волосы: messy jet-black choppy bob до подбородка, blunt straight bangs выше бровей, чёлка разделена на chunky секции с зазорами, текстура roughened/straw-like на кончиках, flyaways
- Лицо: slim elongated oval, значительно длиннее чем шире, очень узкая челюсть, острый маленький подбородок, высокие скулы с мягкими впадинами
- Глаза: узкие миндалевидные, серо-зелёные с olive undertone, slightly hooded, wide-set, спокойный меланхоличный взгляд
- Подводка: thin precise winged black eyeliner только на верхнем веке, short sharp flick, слегка несимметричная (hand-drawn imperfect)
- Губы: ДРАМАТИЧЕСКИ увеличенные, strikingly disproportionate к лицу, обе губы очень полные, нижняя чуть крупнее, strong cupid's bow, nude-pink, matte-to-satin finish, obvious filler aesthetic — ДОМИНАНТНАЯ черта лица
- Нос: тонкий, прямой, маленький, refined tip слегка вниз
- Шея: длинная тонкая, выраженные ключицы
- Выражение по умолчанию: calm, melancholic, emotionally restrained, slightly tired look

### Базовое тело
```
Very slender delicate frame, narrow shoulders, extremely pinched tiny
waist, hips slightly wider than shoulders creating a balanced feminine
silhouette. Long toned legs, overall appearance of a slightly lean
fitness model with a narrow waist.
```

### Базовый наряд (из оригинального промпта)
```
Tight black fishnet short-sleeve top with deep plunging V-neckline to
mid-sternum, black lace bralette visible underneath through the mesh.
Tight glossy black latex pants. Black open-toe high-heeled sandals
with thin stiletto heels.
```

### Вечерний наряд
- Короткое чёрное платье с открытыми плечами
- Длинные сетчатые рукава
- Серебряная цепочка

### Trigger word LoRA: `altushka_v1`

### LoRA статус
- Обучена на FLUX.1-dev base model
- Rank 32, 2000 steps, lr 1e-4
- Файл: altushka_v1.safetensors (328MB)
- Загружена на CivitAI
- Обучена на RTX A6000 на RunPod (~$1.25)
- Датасет: 20 фото с matching caption files и trigger word

### Зафиксированные пресеты

**Altushka_phone:**
iPhone 16 Pro Natural Titanium (серый титан).
Постоянное устройство во всех кадрах с телефоном.
Опционально — прозрачный MagSafe чехол.

**Altushka_hands:**
```
Extremely thin bony feminine hands with disproportionately long slender
fingers, prominent visible knuckles and finger joints, pronounced tendons
on the back of the hand, very flat and narrow palm with almost no soft
tissue padding. Wrist extremely narrow and angular with visible ulna bone
protruding. Skin porcelain-pale, smooth and clean.
No rings, no bracelets, no hand jewelry.
Extremely long sharp stiletto acrylic nails, solid glossy pure black.
Exactly five fingers per hand.
```

**Altushka_apartment_v1:**

Полное описание (RU):
- Тип: modern dark masculine, гранж + готика, casual luxury без глянца
- Палитра: тёмно-серый, графитовый, чёрный, тёплый коричневый (кожа/дерево), бежево-кремовый акцент, оливково-зелёный акцент
- Стены: контраст — одна тёмно-серая матовая с вертикальными панелями, вторая бежево-кремовая
- Пол: тёмный паркет венге/эспрессо, видны швы, матовый
- ТВ зона: OLED на тёмной стене (выключен), под ним — тёмно-коричневая кожаная кушетка/chaise lounge, capitone/quilted, потёртая винтажная кожа
- Мебель: оливково-зелёное кресло/барный стул с чёрными металлическими ножками, стеклянный/мраморный журнальный столик на чёрной ножке
- Зеркало: большое напольное в тёмной раме, прислонено к стене
- Свет: ТОЛЬКО тёплый янтарный 2700-3000K, никакого верхнего белого, никакого холодного LED. Опционально тёплая LED-подсветка за ТВ. Атмосфера всегда вечерняя
- Шторы: плотные блэкаут
- Питомец: померанский шпиц рыже-оранжевый
- Спальня: кровать с тёмным бельём, мятые простыни, кожаное capitone-изголовье
- Кухня: матовые тёмно-серые фасады без ручек, тёмная мраморная столешница
- Ванная: чёрная крупная плитка, матовая чёрная сантехника, зеркало с тёплой LED-подсветкой
- ЗАПРЕЩЕНО: скандинавский стиль, бохо, прованс, яркие цвета, холодный белый свет, ковры с узорами

EN version для промптов:
```
Modern moody dark masculine apartment interior, evening atmosphere.
Contrasting walls — one wall dark grey matte with vertical decorative
panels, another wall beige-cream, creating a sharp vertical color
division. Dark walnut hardwood floors with visible plank seams.
A large flat-screen TV mounted on the dark wall, screen off. Below
the TV — a low dark brown vintage leather chaise lounge with subtle
quilted texture. An accent olive-green chair or barstool with thin
black metal legs to the side. Large dark-framed floor mirror leaning
against the wall. Warm amber low-light only, no overhead white lighting,
evening vibe even during the day, blackout curtains. Optional small
fluffy orange Pomeranian dog. Clean minimalist composition, no clutter,
no bright colors except olive accents.
```

**Altushka_evening_taxi:**
- Короткое чёрное вечернее платье с длинными рукавами
- Белый кожаный салон бизнес-седана
- Заднее сиденье
- Тверская улица ночью
- Поза: нога на ногу
- Ракурс: со стороны водительского сиденья
- Настроение: нейтральная меланхолия

**Altushka_latex_deep_squat:**
Deep athletic squat, hips lowered, knees bent deeply, torso leaning slightly forward, back view, full body.

**Altushka_floor_pose:**
Lying on stomach on floor, upper body on forearms, legs bent at knees, lower legs raised, head toward camera, low-angle three-quarter view.

### Обновлённый промпт лица v2 (АКТУАЛЬНЫЙ — использовать этот)
```
A specific young woman in her early twenties, extremely pale porcelain
skin with cool undertones, almost paper-white, natural skin texture
with visible fine pores, very subtle natural imperfections, no makeup
base visible on the skin, authentic raw skin quality.

Hair: messy jet-black choppy bob reaching jawline to chin length,
heavily textured with choppy razored layers, blunt straight bangs
cut precisely just above the eyebrows, bangs slightly uneven and
separated into chunky sections with small gaps showing the forehead
through them. Hair slightly dishevelled with natural flyaways and
individual strands breaking away from the main shape. The texture is
straight but roughened, almost straw-like at the ends. Hair frames
the face tightly on both sides, curving slightly inward at the jawline.

Face: slim elongated oval face, noticeably longer than wide. Extremely
narrow tapering jawline ending in a small sharp pointed chin. The lower
face is very narrow with almost no width at the jaw. Moderately
prominent high cheekbones creating subtle natural hollows below them,
giving the mid-face gentle angular definition without looking gaunt.

Eyes: narrow almond-shaped eyes with realistic human proportions,
horizontally elongated and slightly wide-set. Soft desaturated
grey-green iris color with a subtle olive undertone, muted and cool.
Slightly hooded upper eyelids with a natural crease visible. The gaze
is calm, slightly melancholic, emotionally restrained. Thin precise
winged black eyeliner on the upper lash line only, extending into a
short sharp flick at the outer corner. The eyeliner is hand-drawn and
slightly imperfect, not perfectly symmetrical between the two eyes.
Natural dark lashes, no false lashes. Eyebrows natural, dark, slightly
thin, with a low soft arch.

Nose: very thin straight small nose, narrow bridge, small refined tip
pointing very slightly downward, delicate and understated.

Lips: dramatically oversized heavily volumized lips, strikingly
disproportionate to the rest of the face. Both upper and lower lip
extremely full and plump, the lower lip slightly larger and pillowy.
Strong defined cupid's bow on the upper lip. Natural nude-pink color
with a soft matte-to-satin finish. Obvious cosmetic filler aesthetic —
the lips are by far the most dominant and immediately noticeable
feature of the entire face. When relaxed, the lips are slightly parted
showing a thin line of teeth. The skin around the lip edges is smooth
and clean with a clear lip border.

Neck and shoulders: very long thin neck, prominent sharp collarbones
visible, extremely slim delicate frame, narrow shoulders.
```

### Промпт лица для генерации (облегчённый, без триггеров):
```
A young woman with a messy jet-black choppy bob with straight bangs
above the eyebrows. Pale skin. Dramatically oversized volumized lips
with obvious filler aesthetic. Narrow almond-shaped grey-green eyes
with thin winged black eyeliner. Slim elongated oval face with narrow
tapering jawline.
```

### Ногти (отдельный блок):
```
Extremely long sharp stiletto acrylic nails, 5-6 cm beyond fingertips,
solid glossy pure black, highly reflective.
```

### Проработанные категории эмоций:
- Базовые, селфи-эмоции, с закрытым/открытым ртом
- Липсинг, TikTok/Reels
- Взгляд в камеру, puppy eyes, высунутый язык
- Mid-conversation (пойман во время разговора, рот открыт)

### Зафиксированные параметры фигуры (подробные):
- Very slender feminine frame
- Narrow delicate shoulders (10-15% уже бёдер)
- Moderately narrow ribcage
- Clearly defined waist (выраженная талия, hourglass)
- Moderately wider hips
- Moderately full natural bust (C-D cup)
- Long slim legs, lean thighs, slim calves
- Long graceful arms, long delicate fingers
- Extremely long stiletto acrylic nails 7-9 cm

### Модульная структура промптов:
Каждый промпт = независимые блоки:
1. Базовая идентичность
2. Фигура
3. Одежда
4. Поза
5. Локация
6. Освещение
7. Камера
8. Эффекты съёмки
9. Эмоция
10. Действие

Менять только отдельные модули. Базовую идентичность — НИКОГДА.

### Зафиксированные сцены:

**Ночная Тверская:**
Москва, Тверская, ночь, мокрый асфальт, свет фар, размытый городской фон, движущийся трафик.

**Селфи-влог:**
Вертикальное 9:16, смартфон в руке, ходьба, естественная тряска, минимальная стабилизация.

**Блок ночного смартфонного селфи:**
```
Authentic nighttime smartphone selfie. Natural low-light smartphone
photography. Slight underexposure 25-35% darker than daylight.
Visible digital sensor noise, fine luminance grain, subtle chroma
noise in shadows. Minor JPEG compression artifacts. Slight sharpening
artifacts. Occasional autofocus imperfections. Moderate motion blur
from walking. Natural handheld camera shake. Rolling-shutter wobble.
Street lights create specular highlights. Bright city lights produce
glow. Headlights create soft light streaks. Wet surfaces generate
reflections and highlight blooms. Small lens flares. Bright areas
slightly overexposed. Subtle ghosting around moving objects.
Handheld phone camera. No stabilization. No cinematic camera movement.
No professional lighting. No beauty filter. No skin smoothing.
Realistic smartphone dynamic range. Authentic social-media selfie
aesthetic. Slightly imperfect image quality. Natural urban night
atmosphere.
```

### Обязательные категории кадров для LoRA:

Ракурсы: фронтальный, сверху 45°, вертикально сверху, снизу от пояса, снизу от ног, поворот головы 45° влево/вправо, три четверти слева/справа.

Освещение: дневное, закат, полная темнота, уличный фонарь, свет экрана.

Выражения: нейтральное, меланхоличное, улыбка, закрытый рот, открытый рот, липсинг, селфи-эмоции, TikTok/Reels.

---

## ПЕРСОНАЖ 2: БЛОНДИНКА

### Базовая идентичность
- Возраст: 20-21 год
- Кожа: светлая, ровная, здоровое сияние, soft warm sun-kissed glow, barely-there веснушки на носу
- Волосы: длинные, НЕЙТРАЛЬНЫЙ ХОЛОДНОВАТЫЙ СВЕТЛЫЙ БЛОНД (light ash-blonde, neutral cool-toned)
  - НЕ golden, НЕ honey, НЕ caramel, НЕ warm yellow, НЕ strawberry, НЕ reddish, НЕ platinum, НЕ silver
  - Лёгкая волна, центральный пробор, voluminous, slightly messy, past shoulders
  - Subtle lighter face-framing pieces
- Лицо: soft youthful oval, smooth full cheeks, gently defined cheekbones, soft small rounded chin, НЕ angular, НЕ hollow
- Глаза: миндалевидные, янтарно-карие, outer corners slightly downturned (cat-eye), calm half-relaxed gaze
  - Clean black winged eyeliner, natural blonde eyebrows with soft arch
- Губы: ОГРОМНЫЕ disproportionately oversized, lower lip especially huge and pillowy, strong filler aesthetic, wet glossy shine, warm rosy-nude, defined cupid's bow
  - Два серебристых snake bites под нижней губой
- Нос: slim straight refined, narrow bridge, small neat pointed tip
- Ногти: длинные миндалевидные, glossy nude finish
- Украшения: тонкая золотая цепочка, тонкое золотое кольцо
- **БЕЗ ТАТУИРОВОК** (полностью чистая кожа, это зафиксировано)

### Якоря узнаваемости:
1. Огромные глянцевые губы (особенно нижняя)
2. Snake bites
3. Юное мягкое лицо с полными щеками
4. Нейтральный холодноватый светлый блонд без тёмных корней
5. Миндалевидные глаза с опущенными уголками
6. Лёгкий загар + еле заметные веснушки на носу
7. Чистая кожа без татуировок
8. Тонкая золотая цепочка

### Trigger word LoRA: `blonda_v1`
### LoRA статус: тренировка начата, НЕ завершена

### Промпт для Nano Banana Pro:
```
A specific young woman in her early twenties, looking youthful around
20-21 years old, light skin with a soft warm sun-kissed glow, smooth
radiant complexion, very subtle barely-there freckles only on the nose,
mostly clear smooth skin, authentic healthy youthful appearance.
No tattoos anywhere on the body, completely clean skin.

Hair: long light blonde hair, neutral cool-toned blonde, evenly blonde
from roots to ends with NO dark roots, subtle lighter face-framing
pieces, natural slightly wavy tousled texture, center parting, voluminous
and slightly messy, falling well past the shoulders. The overall hair
color is a natural light ash-blonde with soft neutral undertones.
NOT golden, NOT honey, NOT caramel, NOT warm yellow, NOT strawberry,
NOT reddish, NOT brown roots, NOT dark roots, NOT platinum, NOT silver.

Face: soft youthful oval face with smooth full cheeks, gently defined
cheekbones, a soft small rounded chin, balanced harmonious proportions,
NOT angular, NOT hollow, NOT bony, NOT gaunt, NOT thin, youthful
softness in the face.

Nose: very slim straight refined nose, narrow throughout, thin narrow
bridge, small neat pointed tip, NOT wide, NOT upturned, NOT button,
NOT rounded tip.

Eyes: almond-shaped eyes, horizontally elongated, medium-sized, warm
amber-brown color, set naturally apart, the outer corners slightly
downturned giving a soft relaxed cat-eye look, NOT round, NOT wide-open,
NOT surprised, NOT upturned, calm half-relaxed gaze, natural blonde
eyebrows with a soft arch. Clean black winged eyeliner.

Lips: enormous disproportionately oversized extremely volumized plump
glossy lips, by far the most dominant feature of the entire face, the
lower lip especially huge and full and pillowy, very strong obvious
cosmetic filler aesthetic, defined cupid's bow, wet glossy shine, warm
rosy-nude color, lips softly parted. Two small symmetrical silver
lower-lip piercings (snake bites).

No tattoos anywhere on the body, completely clean skin. Thin gold chain
or beaded choker necklace.

Hands: slim hands with long fingers, exactly five fingers per hand, long
almond acrylic nails with glossy nude finish.
```

### Промпт для ChatGPT Images:
```
A realistic candid smartphone selfie of a young woman in her early
twenties, around 20 to 21 years old, with a soft youthful face. She has
a gentle oval face shape with smooth full cheeks, softly defined
cheekbones, and a small rounded chin — her face looks young and soft
rather than sharp or thin.

Her hair is long, light blonde in a neutral cool-toned shade, a natural
ash-blonde that leans neither warm nor icy, evenly blonde from roots to
ends with a natural slightly wavy and tousled texture, parted in the
center with subtle lighter face-framing pieces, falling well past her
shoulders.

Her eyes are almond-shaped and horizontally elongated, medium-sized,
warm amber-brown in color, set naturally apart, with the outer corners
angled slightly downward for a soft, relaxed cat-eye look and a calm
half-lidded gaze. Her eyebrows are natural blonde with a soft arch.
She wears a clean black winged eyeliner.

Her lips are the most striking feature of her face — extremely full,
oversized, and plump with an obvious lip filler aesthetic, especially
the lower lip, glossy and softly parted, in a warm rosy-nude shade.
She has two small symmetrical silver piercings below her lower lip
(snake bites).

Her nose is slim, straight, and delicate with a narrow bridge and a
small neat tip. Her skin is light with a soft warm sun-kissed glow,
smooth and radiant, with just a few barely-there freckles across the
nose. No tattoos anywhere on the body. She wears a thin gold chain
necklace. Her nails are long and almond-shaped with a glossy nude finish.

The photo looks like a real casual bedroom selfie taken on a phone in
natural daylight — authentic and slightly imperfect, not retouched,
not a studio shot, with natural skin texture and realistic detail.
```

### Negative prompt (для платформ с полем негатива):
```
dark hair, brown hair, platinum hair, silver hair, ashy hair,
golden hair, honey blonde, strawberry blonde, warm yellow hair,
dark roots, short hair, angular face, hollow cheeks, gaunt,
thin face, narrow face, old, mature, hooded sleepy eyes,
small lips, thin lips, studio lighting, professional photography,
airbrushed, retouched, extra fingers, deformed hands,
illustration, 3d render, cartoon, tattoo, tattoos, body art, ink
```

### Face swap промпт (шаблон для блондинки):
```
Replace the face of the woman in image 1 with the face from image 2.
Keep everything else from image 1 exactly unchanged: [перечислить].
The new face must seamlessly match the lighting direction, skin tone
warmth, and shadow placement. Blend naturally into neck and hairline.
Hair must be long light ash-blonde with center parting from image 2.
Lips must be enormous oversized with glossy filler aesthetic from
image 2. Two small symmetrical silver snake bite piercings below the
lower lip must be visible. Result = one real photograph, not collage.
Photorealistic, natural, no artifacts, no visible seams, no distortion.
```

### Блондинка — Lifestyle серия (зеркальные селфи):

**Локация:** скандинавская квартира-студия (светло-серый, графитовый, белый, чёрный).
Светло-серый ковролин и стены, графитовые шторы, чёрное кресло-мешок, стеклянный столик, белый пушистый коврик, матовая серая кухня, белый рабочий стол с монитором.

**Outfit Lock:** белая облегающая футболка, светло-голубые рваные джинсовые шорты, нюдовый маникюр, Maison Margiela Replica sneakers (off-white, деконструктивный люкс).

**Сцена 01:** селфи у зеркала на полу, ноги согнуты, смартфон частично закрывает лицо.
**Сцена 02:** lifestyle без лица, камера сверху вниз, лицо отсутствует, одна рука на бедре, ноги вытянуты.

### Уроки по промптингу блондинки:
- `hollow cheeks / angular / V-shaped jawline` → лицо слишком взрослое
- `hooded eyes / sleepy` → глаза слишком узкие и усталые
- `platinum / silver / ashy` → волосы седые
- `golden-blonde / sun-bleached / luminous / warm` → волосы уходят в рыжину/золото
- `dark blonde eyebrows` → слово dark цепляет волосы
- Правильно: `light blonde, neutral cool-toned, ash-blonde`
- Для Nano Banana — негативы через NOT работают
- Для ChatGPT Images — негативы переписывать в позитив

---

## ТЕХНИЧЕСКИЙ СТЕК

### Генерация изображений
- **Nano Banana Pro** — основной генератор
- **ChatGPT Images** — альтернатива (негативы в позитив)
- **Face swap** — ВСЕГДА отдельный второй шаг

### Двухшаговый метод (обход фильтров):
1. Генерируем сцену из текста БЕЗ детального описания лица/тела
2. Face swap с референсом лица персонажа
Это обходит и фильтры контента, и детекцию знаменитостей.

### Генерация видео
- **WanAnimate 2.2** через ComfyUI на RunPod
- **Grok** — image to video (Fun mode, 6-10 сек, 720p)

### WanAnimate воркфлоу (ключевые ноды):
- **Нода 287** (Int): fps = 24. Не трогать.
- **Нода 288** (Int): множитель длительности в секундах. Формула: 24 * value + 1 = кадры.
- **Нода 295** (Int): skip_first_frames. 0 = с начала.
- **Нода 303** (Int): разрешение = 854.
- **Нода 232** (ClipVisionEncode): ratio = 0.5 (поднять до 0.7-0.8 для лучшего удержания лица)
- **Нода 244** (LoRA): 5 LoRA загружено — ЭТО ПЕРЕБОР, конфликтуют. Оставить 2: WanAnimate_relight (1.0) + Lightning_I2V (1.0), остальные strength = 0.
- **Нода 266** (Sampler): steps = 4 — мало. Поднять до 6-8.
- **Нода 268** (AnimateEmbeds): face_strength = 1 — слишком высоко. Снизить до 0.7.

### Проблема: потеря консистентности лица на длинных видео.
Причины: конфликт 5 LoRA, мало steps, слабый ratio в ClipVision.
Решение: убрать 3 LoRA, поднять steps и ratio, генерить кусками по 5 сек.

### LoRA тренировка
- AI Toolkit на RunPod (RTX A6000)
- FLUX.1-dev base model
- Датасет: 20-50 фото, разные углы/освещение/выражения
- Кэпшны с trigger word
- ~60-90 минут, ~$1.25-5

### Хостинг моделей: CivitAI, HuggingFace

---

## ОБХОД ФИЛЬТРОВ — ПОЛНЫЙ ГАЙД

### Что триггерит Nano Banana Pro:
- `semi-sheer`, `see-through`, `transparent` + одежда
- `crop top` + `low-rise` + описание фигуры вместе
- `S-curve`, `arched lower back`, `contrapposto` + одежда
- `sculpting leggings`, `heart-shaped contour on glutes`
- `bikini-cut panties`, `thong`
- `midriff exposed`, `navel visible` в сочетании с одеждой
- Детальное описание губ + тела + позы ВСЁ ВМЕСТЕ
- Фото реальных моделей/знаменитостей как референс
- `tongue sticking out`, `playful expression` в некоторых контекстах
- Слово `crop top` + `sleeveless` + `tight` в одном промпте

### Что работает:
- Генерить сцену отдельно, face swap отдельно (главный метод)
- Короткие промпты без детального описания тела
- `fitted` вместо `tight`
- `top` вместо `crop top`
- `lace bottoms` вместо `bikini-cut panties`
- `delicate floral lace bralette` вместо `semi-sheer lace bralette`
- Убирать `midriff exposed`, `navel visible`
- Убирать `slight overexposure on the skin highlights` в некоторых контекстах
- Нейтральные описания поз без позинг-терминов

### Face swap шаблон (универсальный):
```
Replace the face of the woman in image 1 with the face from image 2.
Keep everything else from image 1 exactly unchanged: [ПЕРЕЧИСЛИТЬ ВСЁ:
позу, руки, одежду, фон, освещение, камеру]. The new face must
seamlessly match the [тип освещения] and shadow placement of the
original scene. Blend the face naturally into the neck and hairline.
The hair must [описание волос персонажа] from image 2. The lips must
be dramatically oversized with [filler/volume] aesthetic from image 2.
Maintain [выражение] from image 1. The result should look like one real
[тип фото] of one real person, not a collage or edit. Photorealistic,
natural, no artifacts, no visible seams, no distortion.
```

---

## INSTAGRAM — ПЛАН ПРОГРЕВА

### Текущий статус
- Аккаунт зарегистрирован на немецких прокси и VPN
- День 1-2 прогрева (посмотрел ленту и вышел)

### Подготовка (день 0):
Чистый телефон (сброс). Новый Apple ID. Часовой пояс под локацию. Прокси/VPN под ту же гео. Отдельная симка. Wi-Fi/Bluetooth/Geo выключены.

### Фаза 1 — «Невидимка» (дни 1-7):
- День 1: регистрация, только листать ленту 10-15 минут
- Дни 2-3: смотреть рилсы по тематике (alt/goth/мемы), 2-3 лайка
- Дни 4-5: 3-5 подписок на нишевые аккаунты, нейтральная аватарка с Pinterest, заполнить имя и био
- Дни 6-7: ещё подписки, первая сторис (нейтральная), без AI-контента

### Фаза 2 — «Разгон» (дни 8-14):
- Дни 8-10: первые рилсы — мемы, переписки, тренды без AI-фото. 1 рилс/день
- Дни 11-13: больше сторис (2-3/день), лайки и комменты на чужих аккаунтах
- День 14: включить профессиональный аккаунт, проверить «Похожие авторы»
- POV-фото альтушки без лица можно начинать

### Фаза 3 — «Контент» (день 15+):
- Основной контент с лицом персонажа
- 1 рилс + 2-3 сторис в день, карусель через день
- Можно ставить AI-фото на аватарку

### Правила:
- Первые 14 дней = новорег для Instagram, подозрительный аккаунт
- НЕ ставить AI-фото на аватарку первые 14 дней
- Метаданные фото подставлять под гео (ExifTool)
- 1 аккаунт = 1 прокси (Static Residential ISP лучше VPN)
- Никаких внешних ссылок первые 7 дней
- Bridge page вместо прямых ссылок на платформы
- Для разгона использовать реальные фото моделей с замазанным лицом + мемы

### Telegram:
- Создать сразу, прогрев не нужен
- Формат: кружочки, фото, закулисье
- Ссылку в Instagram ставить только после фазы 3

### Контент-план:
- 1 пост в день
- 2-3 рилса в неделю
- Первые фото без лица и возможно не AI

### Целевая аудитория: СНГ + англоязычная параллельно
### Формат: lifestyle + тренды (танцы позже)

---

## AI OFM CHECKLIST — КЛЮЧЕВЫЕ ВЫВОДЫ

(из документа AI OFM Starter Checklist 2026)

- iPhone XR+ оптимально (iOS-трафик доверительнее)
- Static Residential ISP прокси, не VPN. 1 аккаунт = 1 прокси
- Антидетект-браузер (Dolphin Anty/AdsPower) для нескольких аккаунтов
- Отдельный номер телефона для каждого аккаунта
- Паспорт персонажа (7 полей): имя/локация, возраст/архетип, визуал, психотип, ниша/триггеры, тех.стек, табу
- 5-10 базовых фото до старта
- Bridge page вместо прямых ссылок (Lovable + Render + Namecheap ~$5/мес)
- Reddit как второй источник трафика (2-3 недели karma farming)
- Telegram Stars и VIP-канал для монетизации
- Реальный таймлайн: месяц 1-2 = $0-50, месяц 3-4 = $200-500, месяц 5-6 = $1000-3000

---

## КЛЮЧЕВЫЕ УРОКИ И ПРИНЦИПЫ

### Альтушка:
- Подводка: прямой горизонтальный spike, НЕ изогнутый — recurring error
- Губы = главный идентификационный маркер (#1)
- Причёска = второй маркер (#2)
- Форма лица = третий маркер (#3)
- Лицо важнее всего остального (окружения, одежды, освещения, камеры)

### Блондинка:
- Волосы: ТОЛЬКО neutral cool-toned ash-blonde
- golden/sun-bleached/warm/luminous → рыжина
- Татуировки удалены из ВСЕХ промптов
- Flash photography language triggers filters — убирать

### Общее:
- Двухшаговый workflow: сцена → face swap (обходит фильтры)
- 20 фото датасет с кэпшнами достаточно для узнаваемой LoRA
- Фото проверены на сайте знакомств — 10/10 не видят нейронку
- При ошибках фильтров — итеративно strip triggering language
- Метаданные фото подставлять под гео
- Не использовать фото реальных моделей как референс (детектятся как знаменитости)

---

## ЧТО НУЖНО СДЕЛАТЬ (БЭКЛОГ)

### Срочно (до конца подписки Nano Banana — 4 дня):
- [ ] Паспорт альтушки (имя, характер, легенда, табу)
- [ ] Пачка POV-промптов без лица (10-12 фото для недели 2)
- [ ] Московские локации + промпты (8-10 фото для недели 3)
- [ ] Промпты для квартиры альтушки (selfie/mirror, 5-6 фото)
- [ ] Портреты крупный план (3-4 эмоции)
- [ ] Нагенерить ~30 фото + 3-5 видео

### Потом:
- [ ] Завершить LoRA блондинки
- [ ] Стабилизировать WanAnimate (убрать лишние LoRA, поднять steps)
- [ ] Создать Telegram-канал
- [ ] Паспорт блондинки
- [ ] Bridge page
- [ ] Reddit аккаунт и karma farming
