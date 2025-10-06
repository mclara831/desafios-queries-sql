# A Mensagem do Sensor

- Link do desafio: [A Mensagem do Sensor](https://www.beecrowd.com.br/judge/pt/problems/view/2995)

- **Resolução do desafio**:

![sensor](sensor.png)

- **Solução**:
```sql
select temperature, count(mark) as number_of_records from records 
group by temperature, mark
order by mark
```