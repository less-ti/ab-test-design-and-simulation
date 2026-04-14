# Дизайн A/B-тестов и симуляции

## О проекте

Этот репозиторий посвящен проектированию A/B-тестов для непрерывных метрик и проверке корректности статистических решений с помощью симуляций.

Внутри два отдельных ноутбука:

1. **`ab_test_sample_size_instax.ipynb`** — расчет размера выборки и проверка MDE на данных о продажах.
2. **`nonparametric_ab_test_simulation.ipynb`** — симуляционный подход для случая ненормального распределения и применения непараметрического критерия.

## Используемые данные

В папке `data/` лежат:
- `instax_sales_transactions.csv`
- `ames_housing.txt`

## Структура папки

```text
ab-test-design-and-simulation/
├── README.md
├── README_images.md
├── ab_test_sample_size_instax.ipynb
├── nonparametric_ab_test_simulation.ipynb
├── data/
│   ├── instax_sales_transactions.csv
│   └── ames_housing.txt
└── images/
    ├── instax_metric_distribution.png
    └── bootstrap_sample_means.png
```

## Что сделано

- рассчитан sample size для заданного MDE;
- рассмотрена статистическая мощность теста;
- выполнена проверка через Monte Carlo simulation;
- показан подход к анализу непрерывных метрик при ненормальном распределении.

## Какие навыки показывает проект

- A/B-тестирование;
- power analysis;
- расчет размера выборки;
- проверка гипотез;
- симуляционное моделирование;
- работа с непрерывными метриками.

## Визуализации

![Распределение исторической метрики](images/instax_metric_distribution.png)

![Распределение средних по бутстрап-выборкам](images/bootstrap_sample_means.png)
