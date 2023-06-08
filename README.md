# Aave Liquidity protocol (overview)

### The Aave protocol for decentralised finance (DeFi) enables lending and borrowing of cryptocurrencies and real-world assets (RWAs) without the need for a centralised middleman. They both earn interest from lending and pay it when they borrow.


![image](https://github.com/Holluz/Aave_analysis/assets/128638873/45d54185-27ec-4f16-9bb2-5e82586fd518)


## Methodology

We hope to solve these four main questions

1. Total borrowed on Aave v2
2. Total liquidity supplied on aave v2 
3. Total borrowing per asset
4. Total deposit per asset


![image](https://github.com/Holluz/Aave_analysis/assets/128638873/a2eaaefe-bc6e-4451-87a5-c9c5ccf58c51)

Total Borrowed for Aave V2

Query Code:

```
SELECT SUM(BORROWED_USD/1E9) AS TOTAL_BORROWED  --The total borrowed in billions
FROM ethereum.aave.ez_borrows
WHERE AAVE_VERSION = 'Aave V2'

--AAVE_VERSION Aave V2
```

![image](https://github.com/Holluz/Aave_analysis/assets/128638873/6eb24a88-b6a4-41c6-857f-28efd9aea69a)

Total Supplied for Aave V2

![image](https://github.com/Holluz/Aave_analysis/assets/128638873/0c756f19-00f3-497d-99d3-ddabbc3e912b)

Total borrowed for Aave V2 by Asset

![image](https://github.com/Holluz/Aave_analysis/assets/128638873/34a9f846-4872-4d7a-a447-9d87bd3a6146)

Total Supplied for Aave V2 by Asset





