![linha horizontal](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcltJVGcQCxU3O7Df4woWd_Smrs513ZBzjbWw8nVlE13Z6Ke_2HuCIWIkIVz0NseTTGDGuZ8fGfjY-XyJU2pj6lRCLu5xfETqz0RY3OLKXTf46yMxI58Wp0olynsReeSEYqGAIHbXzdlBjVKtUIZpKzChy1lmSpvYC1dMqckNpupoK6tzZMeQ?key=QvFIoJu-lCkrbQ1nybjL8g)

**Grupo 02 - ODS3 (Saúde e Bem-Estar) - 29/07/2024**

# **Vital+**

**Integrantes:** Clara Araujo Magalhães de Paula, Larissa Scudiere Angioni, Pamela Salgado de Almeida, Paulo Dante Coelho Neto, Tayluan de Jesus dos Santos

Projeto Integrador - Turma Javascript FullStack 05 - Task 4

## **1. OBJETIVO**

Desenvolver a 4ª Task do Projeto Integrador.

**2. DIVISÃO DAS RESPONSABILIDADES** 

| **Integrante**  | **Responsabilidade** |
| --------------- | -------------------- |
| Clara Araújo    | Dev                  |
| Larissa Angioni | Tester               |
| Pamela Salgado  | Dev                  |
| Paulo Dante     | PO                   |
| Tayluan Santos  | Master               |

## **3. DESCRIÇÃO**

**Desenvolvimento**

A quarta task do Projeto Integrador consistiu em desenvolver o CRUD completo da entidade **Categoria,** além de testar seus respectivos métodos.

Para isso, foram desenvolvidas as seguintes classes:

1. **CategoriaService** : Na classe **CategoriaService** foi desenvolvida toda a lógica dos métodos:

- findAll : Lista todas as categorias.
- findById : Busca uma categoria com base no Id passado como parâmetro.
- findByCategoria : Busca uma categoria com base no nome passado como parâmetro.
- create : Cria uma nova categoria no banco de dados. 
- update: Atualiza as informações sobre uma categoria.
- delete: Deleta as informações sobre uma categoria no banco de dados.

1. **CategoriaController:** Na classe **CategoriaController** foi desenvolvida toda a lógica de recebimento das requisições de acordo com o protocolo **HTTP**.

- findAll ( ) - GET / Status Code: 200 OK
- findById - GET / Status Code: 200 OK
- findByCategoria - GET / Status Code: 200 OK
- create - POST / Status Code: 201 CREATED
- update - GET / Status Code: 200 OK
- delete - DELETE / Status Code: 204 NO CONTENT

**Testes**

A parte dos testes foi feita utilizando o Insomnia como ferramenta para realizar as requisições para a API. Todas as requisições atendem no endereço principal **http://localhost:4000/categorias**

**CENÁRIOS POSITIVOS**

**GET - Listar todas as Categorias** 

*http://localhost:4000/categorias*

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdUYaG5RkejGjLDuyXwQ1kJLgxdcb1FJdmcoMBP5exn5jk7Pc5G3sWEUC1K4XylJTk8mOaTN5QsaSxcfBzxilCwyB-XkvB1yZvQTZXRmLHTVOFSrTYzrQjdSX6AdEcorfBgkqmljLXQmJle3YtzKwurNkF4mS0F-PCODDinBw_JBSuMFxbSD-w?key=QvFIoJu-lCkrbQ1nybjL8g)**

**GET ( / {id} ) - Listar Categoria por ID** 

*http://localhost:4000/categorias/{id}* 

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdUYaG5RkejGjLDuyXwQ1kJLgxdcb1FJdmcoMBP5exn5jk7Pc5G3sWEUC1K4XylJTk8mOaTN5QsaSxcfBzxilCwyB-XkvB1yZvQTZXRmLHTVOFSrTYzrQjdSX6AdEcorfBgkqmljLXQmJle3YtzKwurNkF4mS0F-PCODDinBw_JBSuMFxbSD-w?key=QvFIoJu-lCkrbQ1nybjL8g)**

**GET ( /categoria/{categoria} ) - Buscar por Categoria**

*http://localhost:4000/categorias/categoria/{nomeDaCategoria}* 

*![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcv0qWF6zEc3fQNEs0g2ekZhJEGcEIZdHusMHtIa4tY4FEtX4faEu8z5Oz-1028zftcS1FrsVt4f3ILgwtJKXcVSsCZ398Nv9BxQuno8bIwZlnk-usjE5mEvyVuar3SdctBDrRtY4grxUbyjSty1HzMaO1vatEnjV90MPD6lFohlqxf3KfwyZ8?key=QvFIoJu-lCkrbQ1nybjL8g)*

**POST - Criar Categoria** 

*http://localhost:4000/categorias*

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcv0qWF6zEc3fQNEs0g2ekZhJEGcEIZdHusMHtIa4tY4FEtX4faEu8z5Oz-1028zftcS1FrsVt4f3ILgwtJKXcVSsCZ398Nv9BxQuno8bIwZlnk-usjE5mEvyVuar3SdctBDrRtY4grxUbyjSty1HzMaO1vatEnjV90MPD6lFohlqxf3KfwyZ8?key=QvFIoJu-lCkrbQ1nybjL8g)**

**PUT - Atualizar Categoria**

*http://localhost:4000/categorias*

*![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXchYrZ1dR4RaR1njx3Nx0488moB7kpopaYE3pC4b8VRoNqwLnjXjSksNW8D8CI_n--VGl4jAwSTTIXmvJMw4Qmngk1MAzxrELb1A18t24_2ffICqeX9Zql9jNrcBdxKcPWF8x-ciNRveYEEen_Axs2ltjoEwhpYTHjAQkR26zdmvH_vj6fFkw?key=QvFIoJu-lCkrbQ1nybjL8g)*

**DELETE ( /{id} ) - Deletar Categoria**

*http://localhost:4000/categorias/{id}*

*![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe6XlgTC1p200hXIfkSt4npJZDUrphDSATmX4wv5jsM-QO_bKGEWUnLdhaggayvO-Ji6fe9XEAJY9NXKit1MmsQEZ3sg8pQj4ZkjoscD_3WzR5kshSQUU8SEEJQQZVr4odJzQiv0q4baElEPairDFH70d8MS5tkwXBZkzIvL8NK1p1KOBE9tn4?key=QvFIoJu-lCkrbQ1nybjL8g)*

**CENÁRIOS DE ERRO**

**Buscar uma categoria cujo o ID não existe**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXemaALJrSIpGDZBrkjPlvXCfuFlIdeHAudL7gIMzgIYNFUgr3hE0950-cYIexduExwq3lJee1kAu7X4Qlpt2QTxWcmD-7EVKf2Nv04SiUPF1xvi37YTMm86oKWehmUeF1ZHS0pftA8Dmivc2RPIzCsuGg_X0_-yuykb3hWHMYUO3li0j6w2-90?key=QvFIoJu-lCkrbQ1nybjL8g)**

**Cadastrando uma categoria sem passar o atributo “categoria”**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfhMar-DheCdlK1yf8RKrfK7115QHgebtms-tOkRtvkKpO8EMqUWwb3nGbXPD4ZbtC0PaGADVv5tJKAvF6Gdn_s2r1hftcOmE1dwCYmF3Tp806iwxkydN_yKglKZPzQxGISideblOyttCxm_yKosm_0NVq5Ira3Itfy6sRXzUekRA72Me8ceQo?key=QvFIoJu-lCkrbQ1nybjL8g)**

**Atualizando uma categoria sem passar o atributo “categoria”**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdLeIC_mcBXqjnM_-qQ3iyyQKWKdI7su3F7K0gGF07QjDVBbk0vV8MdCNi5aNhNBfXwrtDLbEdVgG1d4GXl05ZCpru_MWO7MJKzxwjz3jCAdRp4SfEiSG9pjD8wR_AVPlqQQPCG2XSEJ-DL8M_79291kevSexaQruSmKeJ23Gynj90YU08Keg?key=QvFIoJu-lCkrbQ1nybjL8g)**

**Atualizando uma categoria cujo o id não existe**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc29NxV-T-9Z6J-7-G7MTNQjLz-4C2eN7tAJqTNcccehdY6E-2Y50HQC7wAZa5hOnXYB35Q-JP-uFrhrBgQLe2D6dSx-DTHfFPcbHjqee2x4P4S13_9F94oEcBW5o6pcyKWufsubyA-6wzrQLe6HQPRGGOP06jLaFvB9TBTuFzIzgoo1QlwBmA?key=QvFIoJu-lCkrbQ1nybjL8g)**

**Deletando uma categoria cujo o id não existe**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcSfKt0dOtC-m9bDoOzwdIQzcHVqtlscVAQGg-1sJQmgVJtWsdOt20Ga-kS9c56xS9hRDQs7p0TucxorCNZGvlnBRuqlqJDDvlm4JL6cw3_991ZtQDYT02QkYjftrol4c61xz2xI-zaJ6h1PPU48siSpalvMIDFSylx6lxXJaEZvD3cHvTGKUQ?key=QvFIoJu-lCkrbQ1nybjL8g)**

**3 - FLUXO GIT - TASK 04****![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdUqnT_ag-mjmM7MPvtQXL3u6NUIcFL3KITM-hck5ht0O04nq72oK-7UVwgdlxSxvEdkT4qdVkVq6zyztRECsp9JT_Qpr1oC92MTluS6OLimdp1AzUkZbgYvBEpngJRlEV8J08_OpgokpIvHFpV31x6ctqCY9Cad9LCE0_VSDwtJbZs5q1Q52M?key=QvFIoJu-lCkrbQ1nybjL8g)**

**4 - LINK DO REPOSITÓRIO**

https://github.com/Projeto-Vital 