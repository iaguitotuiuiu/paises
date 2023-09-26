# paises
Trabalho de Banco de Dados

# INTRO-SQL-BANCO_DE_DADOS
## <p align="left">Trabalho Bimestral de Introdução ao Banco de Dados com SQL por: Paulo Iago Araújo Diogo </p>

### <p align="left">1. Selecione todos os dados dos países da tabela_paises;</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`select * from tabela_paises;`
**<p align="center">CÓDIGO EM IMAGEM</p>**

<div align="center">
  
  ![WhatsApp Image 2023-09-25 at 10 35 06](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/bbed07b3-31b1-4567-84b4-ca62a7d5b658)
</div>

<p align="center">RESULTADO</p>
<div align="center">
  
  ![WhatsApp Image 2023-09-25 at 10 35 06 (1)](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/2e141531-3983-43db-aef3-fc75c806b8bb)
</div>

### <p align="left">2. Selecione todas as cidades cujo país seja brazil;</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`select cidade from tabela_paises where pais = 'Brazil';`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 20](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/b5a8bbd9-5c3d-4e7f-8b71-61ae35425574)
</div>

<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 20 (1)](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/1cb10d65-7452-4dc8-b933-e11b0866a271)
</div>

### <p align="left">3. Selecione todas as cidades cuja região(estado) é ceará;</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`select cidade from tabela_paises where regiao = 'Ceará';`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 29](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/fee7e3c9-c482-4133-8645-3fa8559f80f4)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 29 (1)](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/cd81d47d-5ee5-43a9-8222-eab8de1c768f)
</div>

### <p align="left">4. Utilize a função count para saber quantas regiões(estados) existem na China, 
utilize também o group by;</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`select count(*) as quantidade_regioes, regiao from tabela_paises where pais = 'China' 
group by regiao;`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 38](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/65ddeed6-bf3f-41dd-b17a-9e1cd65f69ca)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 38 (1)](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/09471f3f-b1c6-4fd8-b6cd-42212011f30d)
</div>

### <p align="left">5. Quais regiões, diferentes, existem no Canadá?</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`select distinct regiao, count(*) as quantidade_regioes from tabela_paises where pais = 'Canada'
group by regiao;`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">
  
  ![WhatsApp Image 2023-09-25 at 10 35 48](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/3cf9546a-738a-495a-b003-c19232ce3b9f)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 48 (1)](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/828418db-9ad1-46f3-b4f0-4e7282912903)
</div>

### <p align="left">6. Quantos países diferentes existem na tabela 'tabela_paises';</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`select count (distinct pais) as total_paises
FROM tabela_paises`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 57](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/53894cfa-a937-4333-b10b-577f503ff07e)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 35 57 (2)](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/11380b51-cfeb-4927-9b58-d6aab64d1be4)
</div>

### <p align="left">7. Quantas cidades diferentes existem no brazil;</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`SELECT COUNT(DISTINCT cidade) AS cidade_diferentes FROM tabela_paises where pais = 'Brazil';
`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 07](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/0b84fa5c-fd3c-4405-be73-03130f38de3b)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 08](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/ea888a51-285f-4ccd-afdb-5389a2b1dda0)
</div>

### <p align="left">8. Selecione os países e quantas regiões cada país possui;</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`SELECT pais,COUNT(regiao) AS quantidade_regioes
FROM tabela_paises GROUP BY pais;`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 20](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/ae87606c-c877-428d-b5a6-632a5f7d3f17)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 19](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/dc2a7706-4e73-49a5-b2da-3edbfbbfd08e)
</div>

### <p align="left">9. Quantas pessoas com nome começando em 'João' existem no banco?</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`SELECT COUNT(*) as quantidade_pessoas FROM tabela_paises 
WHERE nome like 'João%';`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 27](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/dc652ba4-995c-4b68-bfdb-f1d8bd6e35a9)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 28](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/4297be51-1ce4-45d8-9506-931adfe2c457)
</div>

### <p align="left">10. Quantas pessoas têm o nome John?</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`SELECT COUNT(*) AS quantidade_john FROM tabela_paises
WHERE nome like 'John%';`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 34](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/a36739d6-c923-4195-9976-f4bbadc6185b)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 34 (1)](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/9b4d70cc-c7f1-4b0c-94b2-035bc51d4644)
</div>

### <p align="left">11. Ordene os nomes dos países sem repetição em ordem alfabética;</p>
**<p align="left">CÓDIGO EM TEXTO</p>**
`select distinct pais from tabela_paises order by pais;`

<p align="center">CÓDIGO EM IMAGEM</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 40](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/de26e54e-d8fb-48a6-9a8e-7b5cd3a3830a)
</div>


<p align="center">RESULTADO</p>
<div align="center">

  ![WhatsApp Image 2023-09-25 at 10 36 41](https://github.com/Kauto22/INTRO-SQL-BANCO_DE_DADOS/assets/111540350/689c3bd1-9501-44e0-ac3f-169a4fd21ed0)
</div>


<div align="center">
  
</div>
