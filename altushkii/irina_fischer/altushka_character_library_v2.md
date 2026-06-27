# Библиотека персонажа «Альтушка» --- цели проекта и зафиксированные пресеты

## Основной замысел проекта

Цель проекта --- создать высококонсистентного оригинального персонажа
(«альтушку») для генерации изображений и обучения LoRA.

Ключевая задача --- добиться того, чтобы персонаж сохранял узнаваемость
между поколениями независимо от:

-   позы;
-   ракурса камеры;
-   одежды;
-   эмоций;
-   освещения;
-   окружения;
-   типа сцены.

Приоритеты проекта:

1.  Максимальная консистентность лица.
2.  Стабильность пропорций тела.
3.  Повторяемость одежды и силуэта.
4.  Корректная работа сложных поз.
5.  Подготовка качественного датасета для LoRA.
6.  Возможность использовать персонажа в фото-, видео- и
    селфи-сценариях.

Основной стек генерации:

-   Nano Banana Pro --- для создания датасета и тестовых генераций.
-   LoRA --- для закрепления идентичности персонажа.
-   Использование модульных блоков: Body, Outfit, Pose, Expression,
    Camera, Scene.

------------------------------------------------------------------------

## Базовая идентичность

-   Возраст: ранние 20 лет.
-   Кожа: очень бледная фарфоровая с холодным подтоном.
-   Волосы: messy jet-black choppy bob, прямые челка выше бровей.
-   Лицо: вытянутое овальное, очень узкая челюсть, острый подбородок.
-   Глаза: узкие миндалевидные, серо-зеленые, тонкая подводка.
-   Губы: очень объемные nude-pink, выраженный filler aesthetic.
-   Нос: тонкий, прямой.

------------------------------------------------------------------------

## База тела

Body: very slender delicate frame, narrow shoulders, extremely pinched
tiny waist, hips slightly wider than shoulders creating a balanced
feminine silhouette. Glutes firm, rounded and athletic, visibly toned
but natural, creating a fit and healthy appearance rather than
exaggerated curves. Thighs slim, lean and proportional, with subtle
athletic definition and no excessive bulk. Long toned legs with elegant
proportions, overall appearance of a slightly lean fitness model with
strong glutes and a narrow waist.

------------------------------------------------------------------------

## Базовый латексный наряд

Outfit: tight black fishnet short-sleeve top with deep plunging
V-neckline to mid-sternum, black lace bralette visible underneath
through the mesh. Tight glossy black latex pants, perfectly fitted to
the legs and hips, emphasizing the athletic lower-body silhouette. Black
open-toe high-heeled sandals with thin stiletto heels.

------------------------------------------------------------------------

## Базовая композиция полного роста

Composition: full body shot, entire body visible from head to feet,
shoes fully visible, standing pose, centered composition, camera
positioned far enough away to capture the complete figure, no cropped
limbs, no cropped feet, full-length portrait.

------------------------------------------------------------------------

## Зафиксированные пресеты

### Altushka_phone — основное мобильное устройство

iPhone 16 Pro в цвете Natural Titanium (серый титан).
Постоянное мобильное устройство альтушки во всех кадрах с телефоном.
Опционально — прозрачный MagSafe чехол.

EN: Natural Titanium grey iPhone 16 Pro, optional clear transparent MagSafe case.

------------------------------------------------------------------------

### Altushka_apartment_v1 — постоянная локация

Тип жилья: современная городская квартира-студия или однокомнатная квартира
в стиле modern dark masculine с гранжевыми и готическими акцентами.
Эстетика — moody, evening vibe, casual luxury без глянца.

**Палитра:**
- Глубокий тёмно-серый, графитовый, угольно-чёрный
- Тёплый коричневый (кожа, дерево)
- Бежево-кремовый акцент (одна стена/панель)
- Зелёный олив как единственный цветной акцент мебели
- Тёплый янтарный свет ламп

**Стены и отделка:**
- Контрастные стены: одна стена тёмно-серая матовая с вертикальными
  декоративными панелями, вторая — светло-бежевая или кремовая.
  Стык создаёт чёткую вертикальную линию-границу.
- Без обоев, без узоров. Только матовая краска.

**Пол:**
- Тёмный деревянный паркет, цвет венге или дуб-эспрессо.
- Видны чёткие швы между планками. Слегка матовая поверхность.

**Зона ТВ:**
- Большой плоский OLED-телевизор на тёмной стене, экран обычно выключен.
- Под телевизором — низкая тёмно-коричневая кожаная кушетка или chaise
  lounge с лёгкой стёганой capitone-текстурой. Кожа потёртая, винтажная.

**Мебель-акценты:**
- Высокий барный стул или кресло оливково-зелёного цвета с тонкими
  чёрными металлическими ножками.
- Стеклянный или мраморный низкий журнальный столик на чёрной ножке.
- Большое напольное зеркало в тёмной деревянной/матово-чёрной раме.

**Освещение:**
- Только тёплый янтарный свет 2700-3000K.
- Никакого верхнего белого света, никакого холодного LED.
- Опционально — тонкая тёплая LED-подсветка за ТВ или по периметру потолка.
- Атмосфера всегда вечерняя, плотные блэкаут-шторы.

**Питомец:**
- Маленький померанский шпиц с рыже-оранжевым окрасом, появляется в кадре.

**Спальня (если в кадре):**
- Кровать с тёмно-серым/антрацитовым постельным бельём, мятые простыни.
- Изголовье из тёмной кожи с capitone-простёжкой.

**Кухня (если в кадре):**
- Матовые тёмно-серые фасады без ручек, тёмная мраморная столешница.

**Ванная (если в кадре):**
- Чёрная плитка крупного формата, матовая чёрная сантехника.
- Большое зеркало с тёплой LED-подсветкой.

**Запрещено:**
- Скандинавский стиль, бохо, прованс.
- Яркие цвета кроме оливки.
- Холодный белый свет, верхний свет.
- Ковры с узорами, подушки с принтами.
- Много живых растений (максимум 1-2 акцента).

**English version for prompts:**

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

------------------------------------------------------------------------

### Altushka_evening_taxi

-   Короткое черное вечернее платье с длинными рукавами.
-   Белый кожаный салон бизнес-седана.
-   Заднее сиденье.
-   Тверская улица ночью.
-   Поза: нога на ногу.
-   Ракурс: со стороны водительского сиденья.
-   Настроение: нейтральная меланхолия.

### Altushka_latex_deep_squat

Deep athletic squat pose with hips lowered significantly, knees bent
deeply, torso leaning slightly forward, natural arch in lower back,
realistic lower-body mechanics, full body visible from head to toe, back
view.

### Altushka_floor_pose

Pose: lying on her stomach on the floor, upper body slightly supported
on forearms or elbows, legs bent at knees and hips, lower legs raised
upward, natural arch through the back, head turned toward the camera,
camera positioned near face side in a low-angle three-quarter view.

------------------------------------------------------------------------

## Проработанные категории эмоций

-   Базовые эмоции.
-   Селфи-эмоции.
-   Эмоции с закрытым ртом.
-   Эмоции с открытым ртом.
-   Липсинг.
-   TikTok / Reels.
-   Взгляд прямо в камеру.
-   Puppy eyes 🥺.
-   Игривые варианты с высунутым языком 😛.

------------------------------------------------------------------------

## Рекомендации по датасету LoRA

-   Сохранять неизменной базовую идентичность.
-   Менять только Scene, Pose, Camera и Expression.
-   Поддерживать разнообразие ракурсов.
-   Использовать крупные планы, средние планы и полный рост.
-   Включать разные позы и сценарии.
-   Следить за консистентностью пропорций.

Целевой результат: LoRA, способная воспроизводить персонажа в любых
новых сценах с сохранением лица, тела и общего визуального стиля.
