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
