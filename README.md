# Мини-проект из урока 6: Анализ взаимодействий с рекламными объявлениями

## Описание проекта

В этом проекте выполняется анализ данных о взаимодействиях с рекламными объявлениями на платформе за период в 6 дней. Задача состоит в исследовании данных, выявлении аномалий, а также в анализе характеристик рекламных клиентов и их конверсии в запуски рекламных объявлений.

## Данные

### Данные взаимодействий с рекламными объявлениями (ads_data.csv)
- **date**: Дата события
- **time**: Время события
- **event**: Тип действия (просмотр или клик)
- **platform**: Платформа
- **ad_id**: Идентификатор объявления
- **client_union_id**: Идентификатор рекламного кабинета
- **campaign_union_id**: Идентификатор рекламной кампании
- **ad_cost_type**: Тип оплаты
- **ad_cost**: Стоимость объявления
- **has_video**: Признак наличия видео в объявлении
- **target_audience_count**: Размер целевой аудитории

### Данные рекламных клиентов (ads_clients_data.csv)
- **date**: Дата взаимодействия
- **client_union_id**: Идентификатор рекламного кабинета
- **community_id**: Идентификатор сообщества
- **create_date**: Дата создания рекламного клиента

## Задачи

1. **Анализ показов и кликов**
   - Вычислите среднее количество показов и кликов на объявления за весь период (округлите до целых).
   - Постройте график распределения показов на объявление за весь период.

2. **Скользящее среднее**
   - Рассчитайте скользящее среднее показов с окном 2. Найдите значение скользящего среднего за 6 апреля 2019 года (округлите до целых).
   
3. **Анализ аномалий**
   - Постройте график, на котором отображены арифметическое среднее по дням и скользящее среднее количества показов.
   - Определите день с наибольшей разницей по модулю между арифметическим и скользящим средними.
   - Напишите функцию, которая определит объявление с наибольшим/наименьшим количеством показов в день с самой значительной аномалией.

4. **Анализ клиентов**
   - Подгрузите данные по рекламным клиентам и найдите среднее количество дней между созданием рекламного клиента и запуском первого объявления.
   - Рассчитайте конверсию из создания рекламного клиента в запуск первой рекламы в течение не более 365 дней. Результат представьте в процентах, округлите до сотых.
   - Разбейте клиентов по промежуткам времени от создания до запуска первого объявления с шагом 30 дней. Подсчитайте количество уникальных клиентов, запустивших первое объявление в первый месяц (от 0 до 30 дней). Используйте промежутки `[0, 30, 90, 180, 365]`.

5. **Интерактивный график**
   - Постройте интерактивный график, показывающий категории клиентов по времени от создания до запуска первого объявления и количество клиентов в каждой категории.

## Выводы

Этот проект помогает выявить закономерности в данных о рекламных кампаниях, а также определить конверсию и поведение клиентов после создания аккаунта. Навыки анализа временных данных и взаимодействия с оконными функциями позволяют получить ценную информацию и визуализировать результаты.


# Mini-Project from Lesson 6: Analysis of Ad Interactions

## Project Description

This project involves analyzing interaction data with advertisements on a platform over a 6-day period. The goal is to explore the data, identify anomalies, and analyze the characteristics of advertising clients and their conversion to launching ad campaigns.

## Data

### Ad Interaction Data (ads_data.csv)
- **date**: Date of the event
- **time**: Time of the event
- **event**: Type of action (view or click)
- **platform**: Platform
- **ad_id**: Advertisement ID
- **client_union_id**: Advertising account ID
- **campaign_union_id**: Advertising campaign ID
- **ad_cost_type**: Payment type
- **ad_cost**: Advertisement cost
- **has_video**: Indicates if the ad contains a video
- **target_audience_count**: Size of the target audience

### Advertising Client Data (ads_clients_data.csv)
- **date**: Date of interaction
- **client_union_id**: Advertising account ID
- **community_id**: Community ID
- **create_date**: Date the client account was created

## Tasks

1. **Analysis of Views and Clicks**
   - Calculate the average number of ad views and clicks over the entire period (round to whole numbers).
   - Create a distribution plot for ad views over the period.

2. **Moving Average**
   - Calculate the moving average of ad views with a window of 2. Find the moving average value for April 6, 2019 (round to whole numbers).

3. **Anomaly Analysis**
   - Create a chart showing the daily arithmetic mean and moving average of ad views.
   - Identify the day with the greatest absolute difference between the arithmetic mean and moving average.
   - Write a function to identify the ad with the highest/lowest number of views on the day of the most significant anomaly.

4. **Client Analysis**
   - Load the advertising client data and calculate the average number of days between creating a client account and launching their first ad.
   - Calculate the conversion rate from client creation to launching their first ad within 365 days. Present the result as a percentage rounded to two decimal places.
   - Categorize clients based on the time intervals from account creation to their first ad launch in increments of 30 days. Count the unique clients who launched their first ad within the first month (0 to 30 days). Use intervals `[0, 30, 90, 180, 365]`.

5. **Interactive Chart**
   - Create an interactive chart showing client categories based on time intervals from account creation to first ad launch and the number of clients in each category.

## Conclusions

This project highlights patterns in advertising campaign data and identifies conversion rates and client behaviors post-account creation. Skills in analyzing time-series data and working with window functions provide valuable insights and help visualize the results effectively.
