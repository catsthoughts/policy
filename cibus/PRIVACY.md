# Политика конфиденциальности Cibus / Cibus Privacy Policy

**Дата вступления в силу / Effective date:** 2025-09-11

_Русская версия ниже. English version below._

---

## Русская версия

### Кто мы

Cibus — приложение для учёта питания и рекомендаций по нутрициологии. Разработчик: Evghenii Chilimciuc (далее — «мы»). Контакт: **echilimciuc@gmail.com**.

Эта политика описывает, какие данные приложение обрабатывает и как. Мы придерживаемся принципа «данные остаются на устройстве»: у Cibus **нет собственных серверов**, нет регистрации и нет облачной синхронизации.

### Какие данные вы вводите и где они хранятся

Все ваши данные хранятся **только локально на вашем устройстве** (в хранилище приложения и в общей группе для виджета). Мы к ним доступа не имеем. Категории данных:

- **Профиль и показатели здоровья:** вес, рост, возраст, пол, уровень активности, тип телосложения, цель, тип диеты.
- **Приём БАДов и лекарств:** списки добавок и лекарственных препаратов, которые вы вносите вручную, и отметки об их приёме.
- **Дневник питания:** съеденные продукты, объёмы, калории и БЖУ, вода, история за период (по умолчанию до 400 дней), избранные продукты.
- **Тренировки и напоминания:** план тренировок, настройки напоминаний (в т.ч. время взвешивания).
- **Настройки приложения:** язык интерфейса, конфигурация AI-ассистента.

Фотографии блюд **не сохраняются** приложением: в дневнике остаётся лишь пометка, что запись создана по фото, и оценка уверенности распознавания.

### Разрешения устройства

- **Камера** — чтобы сфотографировать блюдо для распознавания.
- **Доступ к фото (чтение)** — чтобы выбрать готовое фото блюда.
- **Сохранение в фото (запись)** — чтобы при желании сохранить фото блюда в галерею.
- **Уведомления** — чтобы отправлять напоминания (о приёме пищи, воде, взвешивании и т. п.).

Приложение **не использует** геолокацию, HealthKit, рекламные идентификаторы (IDFA) и не запрашивает эти разрешения.

### Распознавание фото

Распознавание блюда по фото может работать двумя способами:

1. **Локально на устройстве** (по умолчанию) — с помощью встроенной модели машинного обучения (CoreML/Vision). В этом случае изображение **не покидает устройство**.
2. **Через внешний AI-сервис** — только если вы явно включили AI-ассистента и запросили распознавание через него. В этом случае фотография отправляется провайдеру (см. следующий раздел).

### Передача данных внешним AI-сервисам

AI-ассистент по умолчанию **выключен**. Если вы его включаете, при выполнении запросов данные передаются напрямую выбранному AI-провайдеру для обработки запроса. У Cibus нет промежуточного сервера — данные не проходят через нашу инфраструктуру.

**Что может передаваться в запросе:**

- текст с описанием съеденного (названия продуктов, объёмы, калории и БЖУ, цели);
- показатели профиля и здоровья: пол, возраст, вес, рост, ИМТ, телосложение, уровень активности, цель, диета, а также **списки БАДов и лекарств** и план тренировок — они используются, чтобы рекомендации были персональными;
- фотографии блюд (в формате JPEG, закодированные в base64) — только при облачном распознавании фото.

**Куда передаётся (в зависимости от режима):**

- **Бесплатная бета:** запросы идут в OpenRouter (`openrouter.ai`), который направляет их модели DeepSeek. В бета-режиме используется управляемый ключ доступа разработчика — то есть на стороне OpenRouter обращения проходят под учётной записью разработчика, но сами данные обрабатываются сторонними AI-провайдерами, а не Cibus.
- **Свой провайдер (custom):** вы указываете собственный API-ключ, и запросы идут напрямую выбранному вами провайдеру. Поддерживаются: OpenRouter (`openrouter.ai`), DeepSeek (`api.deepseek.com`), OpenAI (`api.openai.com`), Anthropic (`api.anthropic.com`).

Обработка данных этими провайдерами регулируется **их** политиками конфиденциальности:

- OpenRouter — https://openrouter.ai/privacy
- DeepSeek — https://cdn.deepseek.com/policies/en-US/deepseek-privacy-policy.html
- OpenAI — https://openai.com/policies/privacy-policy
- Anthropic — https://www.anthropic.com/legal/privacy

Ваш API-ключ (в режиме «свой провайдер») хранится только на устройстве и используется исключительно для авторизации ваших запросов к провайдеру.

### Аналитика, трекинг и реклама

Приложение **не содержит** аналитики, трекинга, крэш-репортинга, рекламных сетей и сторонних SDK. Мы **не отслеживаем** вас между приложениями и сайтами и **не собираем** ваши данные на своих серверах.

### Экспорт данных

Функция экспорта отчёта формирует обычный текст и помещает его в буфер обмена устройства для ручной вставки вами. Никакой сетевой передачи при экспорте не происходит.

### Удаление данных

Поскольку все данные хранятся локально, вы можете удалить их, очистив данные приложения в его настройках или удалив приложение с устройства.

### Дети

Приложение не предназначено для детей младше 13 лет и не собирает намеренно их данные.

### Медицинский дисклеймер

Cibus предоставляет справочную информацию о питании и рекомендации, в том числе сформированные искусственным интеллектом. Это **не является медицинской консультацией, диагнозом или назначением лечения**. Перед изменением рациона, приёмом БАДов или лекарств проконсультируйтесь с квалифицированным специалистом.

### Изменения политики

Мы можем обновлять эту политику. Актуальная версия всегда доступна по этому адресу; дата вступления в силу указана вверху.

### Контакты

Вопросы по конфиденциальности: **echilimciuc@gmail.com**.

---

## English version

### Who we are

Cibus is a nutrition tracking and dietary guidance app. Developer: Evghenii Chilimciuc ("we"). Contact: **echilimciuc@gmail.com**.

This policy explains what data the app processes and how. We follow an "on‑device" approach: Cibus has **no servers of its own**, no sign‑up, and no cloud sync.

### What you enter and where it is stored

All your data is stored **only locally on your device** (in the app's storage and in an App Group shared with the widget). We have no access to it. Categories:

- **Profile and health metrics:** weight, height, age, sex, activity level, body type, goal, diet type.
- **Supplements and medications:** lists of supplements and medications you enter manually, and intake records.
- **Food diary:** foods eaten, amounts, calories and macros, water, history over time (up to ~400 days by default), favourite foods.
- **Workouts and reminders:** workout plan, reminder settings (including weigh‑in time).
- **App settings:** interface language, AI assistant configuration.

Meal photos are **not stored** by the app: the diary only keeps a note that an entry was created from a photo and the recognition confidence.

### Device permissions

- **Camera** — to photograph a dish for recognition.
- **Photo library (read)** — to pick an existing photo of a dish.
- **Add to photo library (write)** — to optionally save a dish photo to your gallery.
- **Notifications** — to send reminders (meals, water, weigh‑in, etc.).

The app does **not** use location, HealthKit, or advertising identifiers (IDFA), and does not request those permissions.

### Photo recognition

Recognising a dish from a photo can work in two ways:

1. **On device** (default) — using a built‑in machine‑learning model (CoreML/Vision). The image **never leaves your device**.
2. **Via an external AI service** — only if you explicitly enable the AI assistant and request cloud recognition. In that case the photo is sent to the provider (see next section).

### Sharing data with external AI services

The AI assistant is **off by default**. If you enable it, requests are sent directly to the AI provider you use, to fulfil the request. Cibus has no intermediary server — data does not pass through our infrastructure.

**What a request may include:**

- text describing what you ate (food names, amounts, calories and macros, goals);
- profile and health metrics: sex, age, weight, height, BMI, body type, activity level, goal, diet, plus **lists of supplements and medications** and your workout plan — used to make guidance personal;
- meal photos (JPEG, base64‑encoded) — only for cloud photo recognition.

**Where it is sent (depending on mode):**

- **Free beta:** requests go to OpenRouter (`openrouter.ai`), which routes them to a DeepSeek model. In beta the developer's managed access key is used — so on OpenRouter's side requests run under the developer's account, but the data itself is processed by third‑party AI providers, not by Cibus.
- **Your own provider (custom):** you supply your own API key and requests go directly to the provider you choose. Supported: OpenRouter (`openrouter.ai`), DeepSeek (`api.deepseek.com`), OpenAI (`api.openai.com`), Anthropic (`api.anthropic.com`).

Processing by these providers is governed by **their** privacy policies:

- OpenRouter — https://openrouter.ai/privacy
- DeepSeek — https://cdn.deepseek.com/policies/en-US/deepseek-privacy-policy.html
- OpenAI — https://openai.com/policies/privacy-policy
- Anthropic — https://www.anthropic.com/legal/privacy

Your API key (in "your own provider" mode) is stored only on your device and is used solely to authorise your requests to the provider.

### Analytics, tracking, and ads

The app contains **no** analytics, tracking, crash reporting, ad networks, or third‑party SDKs. We do **not** track you across apps and websites and do **not** collect your data on any servers.

### Data export

The report export feature produces plain text and places it on the device clipboard for you to paste manually. No network transmission occurs during export.

### Deleting your data

Because all data is stored locally, you can delete it by clearing the app's data in its settings or by removing the app from your device.

### Children

The app is not directed at children under 13 and does not knowingly collect their data.

### Medical disclaimer

Cibus provides nutritional reference information and guidance, including AI‑generated suggestions. This is **not medical advice, diagnosis, or treatment**. Consult a qualified professional before changing your diet or taking supplements or medications.

### Changes to this policy

We may update this policy. The current version is always available at this address; the effective date is shown at the top.

### Contact

Privacy questions: **echilimciuc@gmail.com**.
