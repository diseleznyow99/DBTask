
# Задачи на работу с базами данных

## Описание проекта

Данный репозиторий представляет собой набор SQL-скриптов для решения задач по работе с базами данных, выполненных с использованием PostgreSQL. Каждая задача представляет собой отдельную часть работы, включающую создание таблиц, заполнение их данными и выполнение SQL-запросов для решения поставленных задач. Проект состоит из четырех основных частей, каждая из которых реализует конкретное задание.


## Структура репозитория
Структура организована следующим образом: для каждой задачи создана отдельная папка, в которой находятся соответствующие SQL-скрипты:

```
.
|   README.md
|
+---task1
|       Task1_0.sql
|       Task1_1.sql
|       Task1_2.sql
|
+---task2
|       Task2_0.sql
|       Task2_1.sql
|       Task2_2.sql
|       Task2_3.sql
|       Task2_4.sql
|       Task2_5.sql
|
+---task3
|       Task3_0.sql
|       Task3_1.sql
|       Task3_2.sql
|       Task3_3.sql
|
\---task4
        Task4_0.sql
        Task4_1.sql
        Task4_2.sql
        Task4_3.sql
```
- В каждой папке задачи сначала размещен скрипт `TaskX_0.sql`, который создает таблицы и наполняет их данными. Эти скрипты не создают базу данных — ее необходимо создать вручную.
- После выполнения скрипта `TaskX_0.sql` можно выполнить последующие файлы, которые содержат SQL-запросы для решения конкретных задач.

## Инструкция по запуску проекта

1. **Создайте базу данных в PostgreSQL.** Пример команды для создания базы данных:
   ```sql
   CREATE DATABASE mydatabase;
   ```

2. **Подключитесь к базе данных.** Например:
   ```bash
   psql -U postgres -d mydatabase
   ```

3. **Создайте таблицы и заполните их данными.** Запустите скрипт `TaskX_0.sql` из папки, соответствующей задаче. Этот скрипт создаст все необходимые таблицы и заполнит их данными.

4. **Выполните решение задачи.** После того как таблицы будут созданы и наполнены, можно запускать последующие скрипты для выполнения конкретных SQL-запросов, например:
   ```sql
   \i task1/Task1_1.sql
   ```


## Описание задач

Все задачи соответствуют исходному техническому заданию

## Примечания

1. Для выполнения SQL-скриптов необходимо иметь доступ к PostgreSQL и создать базу данных вручную.
2. Скрипты создают только таблицы и наполняют их данными, но не создают саму базу данных.
3. Каждая задача решается с использованием SQL-запросов, которые должны быть выполнены последовательно, начиная с `TaskX_0.sql`.
