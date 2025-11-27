# 🎯 Финальный проект по Deep Learning

## 📋 Общая информация

Финальный проект — это ваша возможность применить полученные знания для решения интересной задачи Deep Learning. Проект выполняется индивидуально.

**Максимальная оценка:** 10 баллов  
**Вес в итоговой оценке:** 25% (формула: 0.25×квизы + 0.25×ДЗ + 0.25×экзамен + 0.25×проект)

## 🗓️ Дедлайны и множители

### Важные даты

| **30 ноября** | Репозиторий с экспериментами | −0.25 к множителю |
| **11 декабря** | Защита проекта | Финальная оценка |

### Система множителей

**Базовый множитель:** 1.0

Множитель уменьшается при пропуске дедлайнов:
- Не сдан репозиторий с минимальными экспериментами и бейзлайном до 30 ноября → множитель становится **0.75**

## 🎨 Идеи проектов

### Выбирайте задачу, которую мы НЕ проходили на курсе!

Мы уже делали:
- ❌ Классификацию изображений (CIFAR10, FashionMNIST)
- ❌ Простые полносвязные сети
- ❌ Базовые CNN

Будем делать
- Классификацию изображений с дообучением
- Генерацию простых текстов
- Классификацию текстовых последовательностей

---

## 🖼️ Computer Vision

### 1. Семантическая сегментация изображений 🎯

**Описание:** Разметка каждого пикселя изображения (к какому классу он относится)

**Датасеты:**
- [Cityscapes](https://www.cityscapes-dataset.com/) — сегментация улиц (автомобили, пешеходы, дороги)
- [COCO-Stuff](https://github.com/nightrome/cocostuff) — сегментация 91 класса объектов
- [Pascal VOC](http://host.robots.ox.ac.uk/pascal/VOC/) — классический датасет для сегментации
- [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/) — сегментация сцен (150+ классов)
- [Kaggle Carvana Image Masking](https://www.kaggle.com/c/carvana-image-masking-challenge) — сегментация автомобилей

**Архитектуры:** U-Net, DeepLab, Mask R-CNN, SegNet

**Сложность:** ⭐⭐⭐

---

### 2. Детекция объектов 📦

**Описание:** Найти все объекты на изображении и обвести их bounding box'ами

**Датасеты:**
- [COCO Detection](https://cocodataset.org/) — 80 классов объектов
- [Open Images](https://storage.googleapis.com/openimages/web/index.html) — 600 классов объектов
- [Pascal VOC](http://host.robots.ox.ac.uk/pascal/VOC/) — детекция 20 классов
- [Kaggle Facial Keypoint Detection](https://www.kaggle.com/c/facial-keypoints-detection) — детекция лиц и ключевых точек

**Архитектуры:** YOLO, Faster R-CNN, SSD, RetinaNet

**Сложность:** ⭐⭐⭐⭐

---

### 3. Генерация изображений (GAN) 🎭

**Описание:** Обучение генеративной модели для создания новых изображений

**Датасеты:**
- [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) — 200k фотографий лиц знаменитостей
- [LSUN](https://www.yf.io/p/lsun) — сцены спален, церквей, конференц-залов
- [Anime Face Dataset](https://www.kaggle.com/datasets/splcher/animefacedataset) — лица аниме-персонажей
- [Pokemon Dataset](https://www.kaggle.com/datasets/kvpratama/pokemon-images-dataset) — генерация покемонов

**Архитектуры:** DCGAN, StyleGAN, Pix2Pix, CycleGAN

**Сложность:** ⭐⭐⭐⭐⭐

---

### 4. Super Resolution 🔍

**Описание:** Увеличение разрешения изображений с помощью нейросетей

**Датасеты:**
- [DIV2K](https://data.vision.ee.ethz.ch/cvl/DIV2K/) — 1000 изображений в высоком разрешении
- [Set5, Set14, BSD100](https://github.com/jbhuang0604/SelfExSR) — бенчмарки для super resolution
- [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) — можно downscale и восстанавливать

**Архитектуры:** SRCNN, ESRGAN, EDSR, Real-ESRGAN

**Сложность:** ⭐⭐⭐⭐⭐

---

### 5. Style Transfer 🎨

**Описание:** Перенос стиля одного изображения на другое (например, сделать фото в стиле Ван Гога)

**Датасеты:**
- [WikiArt](https://www.wikiart.org/) — картины художников
- [COCO](https://cocodataset.org/) — обычные фотографии для контента
- Можно использовать любые изображения!

**Архитектуры:** Neural Style Transfer, Fast Style Transfer, AdaIN

**Сложность:** ⭐⭐⭐

---

### 6. Распознавание эмоций 😊😢😠

**Описание:** Классификация эмоций по изображению лица

**Датасеты:**
- [FER-2013](https://www.kaggle.com/datasets/msambare/fer2013) — 35k изображений с 7 эмоциями
- [AffectNet](http://mohammadmahoor.com/affectnet/) — 1M изображений с аннотациями
- [RAF-DB](http://www.whdeng.cn/raf/model1.html) — Real-world Affective Faces

**Архитектуры:** ResNet, VGG, EfficientNet + Transfer Learning

**Сложность:** ⭐⭐

---

### 7. Pose Estimation 🤸

**Описание:** Определение позы человека (положение ключевых точек тела)

**Датасеты:**
- [MPII Human Pose](http://human-pose.mpi-inf.mpg.de/) — 25k изображений с аннотациями
- [COCO Keypoints](https://cocodataset.org/#keypoints-2020) — детекция ключевых точек
- [Human3.6M](http://vision.imar.ro/human3.6m/) — 3D позы

**Архитектуры:** OpenPose, HRNet, PoseNet

**Сложность:** ⭐⭐⭐⭐

---

## 🗣️ Natural Language Processing

### 8. Генерация заголовков для изображений (Image Captioning) 📝

**Описание:** Автоматическое создание текстового описания изображения

**Датасеты:**
- [COCO Captions](https://cocodataset.org/#captions-2015) — 330k изображений с 5 описаниями каждое
- [Flickr30k](http://shannon.cs.illinois.edu/DenotationGraph/) — 31k изображений
- [Conceptual Captions](https://ai.google.com/research/ConceptualCaptions/) — 3.3M пар изображение-текст

**Архитектуры:** CNN + LSTM/Transformer, Show and Tell, BLIP

**Сложность:** ⭐⭐⭐⭐⭐

---

### 9. Генерация текста 📖

**Описание:** Обучение языковой модели для генерации текста (стихи, истории, код)

**Датасеты:**
- [WikiText](https://blog.salesforceairesearch.com/the-wikitext-long-term-dependency-language-modeling-dataset/) — статьи из Wikipedia
- [BookCorpus](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Zhu_Aligning_Books_and_ICCV_2015_paper.pdf) — 11k книг
- [Russian Poetry](https://www.kaggle.com/datasets/yakorch/russian-poetry-corpus) — русские стихи
- [GitHub Code Dataset](https://www.kaggle.com/datasets/github/github-repos) — код на Python/JS

**Архитектуры:** GPT-2, LSTM, Transformer

**Сложность:** ⭐⭐⭐⭐

---

### 10. Named Entity Recognition (NER) 🏷️

**Описание:** Выделение в тексте имен людей, организаций, локаций и т.д.

**Датасеты:**
- [CoNLL-2003](https://www.clips.uantwerpen.be/conll2003/ner/) — английский NER
- [OntoNotes 5.0](https://catalog.ldc.upenn.edu/LDC2013T19) — 18 типов entities
- [Russian NER](https://www.kaggle.com/datasets/raenish/russian-ner) — русскоязычный NER

**Архитектуры:** BiLSTM-CRF, BERT + CRF, SpaCy

**Сложность:** ⭐⭐⭐

---

## 🎵 Audio & Speech

### 11. Распознавание речи (Speech Recognition) 🎤

**Описание:** Преобразование аудио в текст

**Датасеты:**
- [LibriSpeech](https://www.openslr.org/12/) — 1000 часов английской речи
- [Common Voice](https://commonvoice.mozilla.org/) — мультиязычный датасет (есть русский!)
- [TIMIT](https://catalog.ldc.upenn.edu/LDC93S1) — фонетическая транскрипция

**Архитектуры:** DeepSpeech, Wav2Vec 2.0, Whisper

**Сложность:** ⭐⭐⭐⭐

---

### 12. Классификация музыкальных жанров 🎵

**Описание:** Определение жанра музыкальной композиции

**Датасеты:**
- [GTZAN](https://www.kaggle.com/datasets/andradaolteanu/gtzan-dataset-music-genre-classification) — 1000 треков, 10 жанров
- [FMA (Free Music Archive)](https://github.com/mdeff/fma) — 106k треков
- [Million Song Dataset](http://millionsongdataset.com/) — метаданные миллиона песен

**Архитектуры:** CNN на спектрограммах, CRNN, Audio Transformers

**Сложность:** ⭐⭐⭐

---

### 13. Распознавание эмоций в голосе 🎭🗣️

**Описание:** Определение эмоции говорящего по аудиозаписи

**Датасеты:**
- [RAVDESS](https://www.kaggle.com/datasets/uwrfkaggle/ravdess-emotional-speech-audio) — эмоциональная речь
- [CREMA-D](https://www.kaggle.com/datasets/ejlok1/cremad) — 7k эмоциональных клипов
- [SAVEE](http://kahlan.eps.surrey.ac.uk/savee/) — британский английский

**Архитектуры:** CNN + LSTM на mel-спектрограммах

**Сложность:** ⭐⭐⭐

---

## 🤖 Другие интересные задачи

### 14. Рекомендательная система 🎬

**Описание:** Предсказание рейтинга или рекомендация фильмов/товаров

**Датасеты:**
- [MovieLens](https://grouplens.org/datasets/movielens/) — 25M рейтингов фильмов
- [Netflix Prize Dataset](https://www.kaggle.com/datasets/netflix-inc/netflix-prize-data) — 100M рейтингов
- [Amazon Reviews](https://www.kaggle.com/datasets/skillsmuggler/amazon-ratings) — отзывы на товары

**Архитектуры:** Matrix Factorization, Neural Collaborative Filtering, Autoencoders

**Сложность:** ⭐⭐⭐

---

### 15. Прогнозирование временных рядов 📈

**Описание:** Предсказание будущих значений (цены акций, погода, трафик)

**Датасеты:**
- [Stock Market Data](https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs) — исторические цены акций
- [Bike Sharing](https://www.kaggle.com/datasets/lakshmi25npathi/bike-sharing-dataset) — прокат велосипедов
- [Energy Consumption](https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption) — потребление электроэнергии

**Архитектуры:** LSTM, GRU, Transformer (Temporal Fusion Transformer)

**Сложность:** ⭐⭐⭐

---

### 16. Игровой AI 🎮

**Описание:** Обучение агента играть в игру с помощью Reinforcement Learning

**Среды:**
- [OpenAI Gym](https://gymnasium.farama.org/) — CartPole, Atari games
- [Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents) — 3D среды
- Собственная игра (Snake, Flappy Bird, etc.)

**Алгоритмы:** DQN, PPO, A3C, DDPG

**Сложность:** ⭐⭐⭐⭐⭐

---

## 📝 Требования к проекту

### Обязательные компоненты

1. **README.md** с описанием:
   - Постановка задачи
   - Описание датасета
   - Архитектура модели
   - Результаты (метрики, графики)
   - Примеры работы модели
   - Инструкция по запуску

2. **Код:**
   - Загрузка и предобработка данных
   - Определение модели
   - Обучение с логированием метрик
   - Визуализация результатов
   - Inference на новых данных

3. **Эксперименты:**
   - Минимум 3 разных эксперимента (архитектуры, гиперпараметры, аугментации)
   - Сравнение результатов

4. **Визуализации:**
   - Графики обучения (loss, метрики)
   - Примеры предсказаний модели
   - Confusion matrix / другие визуализации качества

### Критерии оценивания

| Критерий | Баллы |
|----------|-------|
| Корректность реализации | 3 |
| Качество кода и документации | 2 |
| Эксперименты и анализ | 2 |
| Визуализация результатов | 1 |
| Качество модели (метрики) | 1 |
| Презентация на защите | 1 |

### Дополнительные баллы (бонусы)

- +0.5 за использование Transfer Learning
- +1 за деплой модели (Streamlit/Gradio/Telegram bot)
- +0.5 за особо креативное решение

---

## 🚀 Советы по выполнению

1. **Начните с простого baseline** — простая модель лучше, чем сложная, но нерабочая
2. **Используйте Google Colab** — бесплатный GPU поможет быстрее обучать модели
3. **Transfer Learning — ваш друг** — предобученные модели экономят время
4. **Логируйте всё** — используйте TensorBoard, Weights & Biases или просто сохраняйте метрики
5. **Сравнивайте с baseline** — всегда есть простое решение для сравнения
6. **Документируйте процесс** — README пишется параллельно с кодом, а не в последний день
7. **Делайте коммиты регулярно** — git history показывает ваш прогресс

---

## 📬 Сдача проекта

### Промежуточная сдача (до 30 ноября включительно)

Создайте **публичный** GitHub репозиторий, который содержит:
- ✅ README с описанием задачи и планом
- ✅ Код загрузки и анализа данных
- ✅ Хотя бы один работающий baseline
- ✅ Первые эксперименты

Отправьте ссылку на репозиторий в [форму](https://forms.gle/R6PndMUV8tLj7Rax8)

### Защита (4 декабря)

Подготовьте:
- **Презентация** (5-7 минут):
  - Задача и мотивация
  - Данные
  - Подход и архитектура
  - Результаты и визуализации
  - Выводы
- **Демонстрация** — покажите работу модели на примерах
- **Код** — будьте готовы ответить на вопросы по коду

---

## 💡 Полезные ресурсы

- [Papers with Code](https://paperswithcode.com/) — статьи и код SOTA моделей
- [Kaggle](https://www.kaggle.com/) — датасеты и примеры решений
- [Hugging Face](https://huggingface.co/) — предобученные модели
- [PyTorch Tutorials](https://pytorch.org/tutorials/) — официальные туториалы
- [TensorFlow Datasets](https://www.tensorflow.org/datasets) — готовые датасеты


