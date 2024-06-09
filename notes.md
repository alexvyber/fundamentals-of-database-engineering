```SQL
-- fill millions rows with random integers
insert into temp(t) select random() * 100 from generate_series(0, 1_000_000);

-- analyze query
explain analyze select id from table_name where id=42069;
```