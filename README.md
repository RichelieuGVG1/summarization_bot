# <p align="center"> Суммаризация чата и вопрос-ответ</p>



## Оглавление
1. [Задание](#1)
2. [Решение](#2)
3. [Запуск кода](#3)
4. [Стек](#5)


## <a name="1"> Задание </a>

Необходимо разработать бота для телеграмма, который позволяет трекать темы в чате, чтобы человеку не приходилось монотонно листать чат в поисках важной информации.

## <a name="2">Решение </a>

Решение представляет из себя применение одной и той же модели для RAG (но еще 1 ретривер модель) и суммаризации: Saiga llama-3-8b с подобранным промптом для получения стабильного, точного ответа в особенности без галлюцинаций

### Архетиктура модели
<img width="550" height="400" alt="image" src="https://github.com/holopyolo/QAnSummarization_WorkChats/blob/main/images/photo_2024-07-05_06-13-06.jpg"> 

<br>

## <a name="3">Запуск кода </a>

### Последовательные шаги для запуска кода:
1. Сборка;
```Bash
docker build -t my-python-app .
```
2. Запуск;
```Bash
docker run -d --name my-app-container my-python-app
```

## Используем одну ЛЛМ отлично справляющуюся как с задачей RAG, так и суммаризацией. Используем кеширование, чтобы часто не тратить время на генерацию ответа.

## <a name="4">Стек </a>
  <img src="https://github.com/devicons/devicon/blob/master/icons/python/python-original-wordmark.svg" title="Python" alt="Puthon" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/pytorch/pytorch-original.svg" title="Pytorch" alt="Puthon" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/numpy/numpy-original.svg" title="Numpy" alt="Puthon" width="40" height="40"/>&nbsp;
  <img src="https://github.com/gradio-app/gradio/blob/main/readme_files/gradio.svg" title="Gradio" alt="Puthon" width="100" height="40"/>&nbsp;


