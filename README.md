# diagram
```mermaid
flowchart TD
A[Генерация идеи<br/>PM, Delivery] --> B[Описание<br/>(Industrial Analyst)]
B --> C[Структурирование и создание ТЗ<br/>(SA)]
C --> D[Ревью ТЗ<br/>TechLead, Senior SA]
D --> E[Создание задачи в бэклог<br/>SA]
E --> F[Оценка трудозатрат на задачу<br/>(Developer, TechLead)]
F --> G[Принятие задачи на спринт<br/>(Team Lead)]

subgraph "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sprint"
direction TB
G --> H[Назначение ответственного разработчика и исполнение<br/>Team Lead]
H --> I[Проведение необходимых тестов<br/>Developer]
I --> J[Тестирование <br/>SA]
I --> K[Ревью<br/>Thech Lead]
J --> L[В очередь на Деплой<br/>TechLead]
K --> L
end

L --> M[Деплой на прод<br/>DevOps]
M --> N[Перевод на статус Готово<br/>DevOps]
```
