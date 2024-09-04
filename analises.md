## Ranking em SQL
***
```sql
SELECT 
    *,
     DENSE_RANK()
    OVER(
        PARTITION BY estudantes
        ORDER BY nota DESC
    ) AS ranking_notas
FROM pagina1
```
