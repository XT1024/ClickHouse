# Nothing {#nothing}

Этот тип данных предназначен только для того, чтобы представлять [NULL](../../query_language/syntax.md), т.е. отсутствие значения.

Невозможно создать значение типа `Nothing`, поэтому он используется там, где значение не подразумевается. Например, `NULL` записывается как `Nullable(Nothing)` ([Nullable](../../data_types/nullable.md) — это тип данных, позволяющий хранить `NULL` в таблицах). Также тип `Nothing` используется для обозначения пустых массивов:

``` sql
SELECT toTypeName(Array())
```

``` text
┌─toTypeName(array())─┐
│ Array(Nothing)      │
└─────────────────────┘
```

[Оригинальная статья](https://clickhouse.tech/docs/ru/data_types/special_data_types/nothing/) <!--hide-->
