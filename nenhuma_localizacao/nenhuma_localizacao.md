# Nenhuma Localização

Link do desafio: [Nenhuma localização](https://www.beecrowd.com.br/judge/pt/problems/view/2616)

- **Resolução do desafio**:

![nenhuma_localizacao](nenhuma_localizacao.png)

- **Solução**:
```
select c.id, c.name from customers c
where c.id not in (select l.id_customers from locations l) 
order by id;
```