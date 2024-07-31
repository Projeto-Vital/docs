![linha horizontal](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfXyl3ozmsNqPiRk1KPUkq3AuUWxNa8Sux1ZjpqNy02r1q3OcHwcRcbwYX-k1BSaHHPjWs3B5ijn3Rpojy5gEDmHd1d18jUcpdmQWacTclxRDOgQhLvRkABSENniatNhVVVKkp8L2-LnSAcDZ5Yq2ugUpSDLiPNPZzPK72ZjQ6is5iCpOZlyA?key=_061iz5IFcilyWc777QLCQ)

**Grupo 02 - ODS3 (Saúde e Bem-Estar) - 30/07/2024**

**Vital+**

**Integrantes:** Clara Araujo Magalhães de Paula, Larissa Scudiere Angioni, Pamela Salgado de Almeida, Paulo Dante Coelho Neto, Tayluan de Jesus dos Santos

Projeto Integrador - Turma Javascript FullStack 05 - Task 5



## **1. OBJETIVO**

Desenvolver a 5ª Task do Projeto Integrador - Criação da Entidade Produto relacionada com a Entidade Categoria, criação da Classe de Serviço do Produto e criação da Classe Controladora do Produto. Além disso, terá também a criação da Entidade Usuário.



## **2. DIVISÃO DAS RESPONSABILIDADES** 

| **Integrante**  | **Responsabilidade** |
| --------------- | -------------------- |
| Pamela Salgado  | PO                   |
| Larissa Angioni | Dev                  |
| Tayluan Santos  | Tester               |
| Clara Araujo    | Master               |
| Paulo Dante     | Dev                  |



## **3. DESCRIÇÃO**

- Criar a branch **task_05**, para trabalharmos as novas funcionalidades.

- Fazer um clone do repositório remoto para o local 

- Criar a pasta produtos e, nela, suas subpastas, **entidades**, **controllers** e **services** e o arquivo **produto.module.ts** com as importações, exportações, provedores e controladores.

- Criar a Classe **Produto** com seus respectivos atributos e fazer o relacionamento **ManyToOne** com a **Categoria**. 

- Criar a Classe **ProdutoService** com os métodos CRUD.

- Criar a Classe **ProdutoController** com os controles de requisições 

- Testar a aplicação a fim de identificar possíveis erros antes de fazer a integração com branch principal do projeto.

  

## **Testes**

A aplicação foi testada no Insomnia, para realizar as requisições para a API. E todas as requisições atendem no endereço principal [**http://localhost:4000/produtos**](http://localhost:4000/produtos)

### **CENÁRIOS POSITIVOS**

**GET - Listar todos os Produtos**

*http://localhost:4000/produtos*

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdpDz5QsI2v7N-S6QTioeo6pMe7uwxLcvaUB8Et588epubdCqj963rBjV9OeElCwGEvfLI0A8ENfAIchCbhvptHQT1ikp8mtmlaC1o3c20LUSzyT_6K3oyu-SsIhp4MqdjN6xekxQyWxWcS-PoymkviaOUACeeu70NPu7MwoQ?key=_061iz5IFcilyWc777QLCQ)**

**GET ( / {id} ) - Buscar Produto por ID** 

*http://localhost:4000/produto/{id}* 

*![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf7JHyXbjVTVnhYozlQexBBT5D5w30KGRpo_URaByL83ffpKpRSLKY4j5qJjmgnZUmUABnjz7YWkkNWvD7pmf9e18pG20zablm0XoseQvQetr2MhtYgZ62-J5OD_wAH2UwuZa2UdJzF_--GMWSXx3XEEKN3hhCk9paZggCLnw?key=_061iz5IFcilyWc777QLCQ)*

**GET ( /nome/{nome} ) - Buscar por Produto por Nome**

*http://localhost:4000/produtos/nome/{nomeProduto}* 

*![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeR_CDQ5WEShTU0JVkVjhsK_pKn_ypgUSXxUjBcgCfHd3NUhVlhYFM_vjeFDmpdSdRLyntf7RGwoScArix6hIt__wQ9AmqCRvFipXuuWgARsj4dV0iDqNw8BbvmbqwZ4wOOux82ZkEKb-NURAkoKuJKbaRuVYxh7i7CQM49rQ?key=_061iz5IFcilyWc777QLCQ)*

**POST - Criar Produto**

*http://localhost:4000/produtos*

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUm76Qs7Y0ibriBeHco1AmkO2lZ8R_F5GLESYycq3QBHbzsV3keNJEQZDey2Cego3U1_4hTPveRV1kt_pMgH4bccr9_fsyx8XjwP3bkScYojPHNW5kcky5XJpmT4fPpVYPeOvCWSaQYYYRBptIMoRx_cOXqhN6_AaTtua2lQ?key=_061iz5IFcilyWc777QLCQ)**

**PUT - Atualizar Produto**

*http://localhost:4000/produtos*

*![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcdWK5VtMXzXJK2KeGirveUM0G2iKYBc5rM5WJBuXCNxznczh1RdhQOfU-C3mxaO3jjOTfRrzNzMMJenQH3O_SVPPy5mdlXBygrh9Sq-3VU8zNv3N5xYKAmNWe1eWye4H5hHrIH8JGW5Xsa6mHfWhNxBtT0uVzbuTH2ynFOGw?key=_061iz5IFcilyWc777QLCQ)*

**DELETE ( /{id} ) - Deletar Produto**

*http://localhost:4000/produtos/{id}*

*![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcy7kkL9WtWPYOPi9qcTCpgGAh1XLlFBW7h6_3XoQrnziZJNrl_q4a_DC6pb_x6neDr6cAT2V_r6N22pqzqeEfbPCdD5DdwTkZX1_frk5IH5t_bSue6Oev5T1bQMkknyfGCQ3cCQpL201IvduLzRUnqc0E984jbgd-D0efWkw?key=_061iz5IFcilyWc777QLCQ)*

### **CENÁRIOS DE ERRO**

**Buscar um produto cujo o ID não existe**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcx2YvdAHHy73OXFwGRjCaH0gvRIyqD3OuwTYyLxZo4nqNBEdY0tJRmRGmOndWaKzEve9N0L39amO8sklwg3nOUxXn9RToefJh3gU35TLAvup8-bOB2AjrTcLNhZ5cs553zNn32aDPSsblV9EZ71_AHEIAvJkZRd0rf_JQs1Q?key=_061iz5IFcilyWc777QLCQ)**

**Cadastrando um produto sem passar um atributo obrigatório**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeONo_DIfLLElyOfsAFR5gfsXahqTY2Ii6WqRQKIuz9thbTxyppLGbN4C9YxK3ZOLMeoiH8VqaJBC8-hWlAFXz5nwszwdhR1Db2t_vj1J1PVIxdwDSvX7P6k_mIWuSYcszFY7N6lkhyBwbWOdqp-1RaBXhmphYYKsGC76fbzg?key=_061iz5IFcilyWc777QLCQ)**

**Atualizando um produto sem passar um atributo obrigatório**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeONo_DIfLLElyOfsAFR5gfsXahqTY2Ii6WqRQKIuz9thbTxyppLGbN4C9YxK3ZOLMeoiH8VqaJBC8-hWlAFXz5nwszwdhR1Db2t_vj1J1PVIxdwDSvX7P6k_mIWuSYcszFY7N6lkhyBwbWOdqp-1RaBXhmphYYKsGC76fbzg?key=_061iz5IFcilyWc777QLCQ)**

**Atualizando um produto cujo o id não existe**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeKgdXz1q2yx7eZ2DSL7ZjjaT9WRLod6WweJ-QV2y9X_pKtjqa51v7Ht86miVgATNvQ3cCVtelqF1L2Jg-VvDAJCC0VX6JfB6OApb1vp7a5-Z0We-4v4bwX5lPcvel5ZDOufVKhhfr7CFms3ZeIVyeNdvoZsnS9N1ocRFoW?key=_061iz5IFcilyWc777QLCQ)**

**Deletando um produto cujo o id não existe**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeKgdXz1q2yx7eZ2DSL7ZjjaT9WRLod6WweJ-QV2y9X_pKtjqa51v7Ht86miVgATNvQ3cCVtelqF1L2Jg-VvDAJCC0VX6JfB6OApb1vp7a5-Z0We-4v4bwX5lPcvel5ZDOufVKhhfr7CFms3ZeIVyeNdvoZsnS9N1ocRFoW?key=_061iz5IFcilyWc777QLCQ)**

**3 - FLUXO GIT - TASK 05**

**![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXebQ2-2Yq3FhvM12TVQtEmLIzd1VM44GmrLZp7wOgKt7kVqDll-CQpWEfFRLwMUBbxzLhVpvKJgsuR9CeqBs6jWjRJrnzloqOkj9n5XPUftziAPtVQd7O_hMZKPkRg_Xln8a7x6DeRB7KP9Y_dEbLxLFvEsd1GdUuELcucx?key=_061iz5IFcilyWc777QLCQ)**

**4 - LINK DO REPOSITÓRIO**

https://github.com/Projeto-Vital 