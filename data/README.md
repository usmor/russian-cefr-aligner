# Датасет для классификации уровней CEFR

## Обзор датасета
Этот датасет содержит русские тексты с аннотациями уровней Общеевропейской системы уровней владения иностранным языком (CEFR) от A1 до C2, предназначенный для обучения классификаторов уровней CEFR.

Датасет сбалансирован по уровням и разделён на тренировочную, валидационную и тестовую выборки.

---
## Разделение данных

Общая выборка была разделена в следующих пропорциях:

| Выборка     | Количество примеров | % от общего |
|------------|---------------------|-------------|
| Train      | 21 163              | 80.0%       |
| Validation | 2 646               | 10.0%       |
| Test       | 2 645               | 10.0%       |
| **Всего**  | **26 454**          | 100.0%  |

---

## Распределение по уровням

| CEFR | Всего | Train | Validation | Test |
|-----|-------|-------|------------|------|
| A1  | 4 409 | 3 528 | 441        | 440  |
| A2  | 4 409 | 3 527 | 441        | 441  |
| B1  | 4 409 | 3 527 | 441        | 441  |
| B2  | 4 409 | 3 527 | 441        | 441  |
| C1  | 4 409 | 3 527 | 441        | 441  |
| C2  | 4 409 | 3 527 | 441        | 441  |

---

## Источники данных

Итоговый корпус был сформирован путём конкатенации и фильтрации данных из нескольких источников:

### Основные датасеты
- **UniversalCEFR (Russian)**  
  https://huggingface.co/datasets/UniversalCEFR/readme_ru
- **RuAdapt** (сказки и адаптированная литература)  
  https://github.com/Digital-Pushkin-Lab/RuAdapt
- **FluencyDrop** (уровни A1, C1, C2)  
  https://fluencydrop.com/stories/russian

### Литературные произведения (уровни B2–C2)
- Ильф И., Петров Е. — *«12 стульев»*  
  http://az.lib.ru/i/ilfpetrov/text_0100.shtml
- Замятин Е. — *«Мы»*  
  http://az.lib.ru/z/zamjatin_e_i/text_0050.shtml
- Достоевский Ф. — *«Идиот»*  
  https://royallib.com/book/dostoevskiy_fedor/tom_6_idiot.html

### Дополнение для начальных уровней (A1–A2)

Начальные уровни были расширены короткими учебными и адаптированными текстами из ресурсов для изучения РКИ:

- **Stories in Easy Russian. Level A2**  
  https://psv4.userapi.com/s/v1/d/y2llikxq731Sje6eRNxA17pXwNkhXPhZt9T30h1qkOP5a2xvvYKJMtgoeKF0FkjCrnZIcSFfyBRGlHDRBo_yc03ZWSX29xaSHfqFu5HM3t7f6XdD5NvZ_w/1russian_stories_level_a2_book_1.pdf
- **Медиатека учебных текстов ИРЯиК МГУ**  
  https://www.catalogue.irlc.msu.ru/media-texts-catalogue/
- **Курлова И. — «Начинаем читать по-русски!»**  
  https://chamilanguerussepourtous.nethouse.ru/static/doc/0000/0000/0304/304431.3g5ldd472t.pdf
- **On-line Russian language school Pa-russki**  
  https://pa-russki.com
- **AnyLang: перевод книг и видео**  
  https://anylang.net/ru/books

---
