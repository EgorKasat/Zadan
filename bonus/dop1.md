```mermaid
sequenceDiagram
    participant C as Клиент
    participant A as Приложение
    participant R as Ресторан
    participant K as Курьер
    participant S as Сервер

    C->>A: Создание заказа
    A->>S: Отправка заказа
    S->>R: Уведомление о заказе
    R->>S: Подтверждение
    S->>K: Назначение заказа
    K->>R: Забор заказа
    K->>C: Доставка
    C->>A: Подтверждение получения
    A->>S: Обновление статуса