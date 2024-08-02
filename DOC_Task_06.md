**Grupo 02 - ODS3 (Saúde e Bem-Estar) - 02/08/2024**

**Vital+**

**Integrantes:** Clara Araujo Magalhães de Paula, Larissa Scudiere Angioni, Pamela Salgado de Almeida, Paulo Dante Coelho Neto, Tayluan de Jesus dos Santos

# Projeto Integrador - Turma Javascript FullStack 05 -     Task 6



## **1. OBJETIVO**

Desenvolver a 6ª Task do Projeto Integrador - O objetivo desta tarefa é aprimorar a segurança e funcionalidade do projeto.

## **2. DIVISÃO DAS RESPONSABILIDADES** 

| **Integrante**  | **Responsabilidade** |
| --------------- | -------------------- |
| Larissa Angioni | PO                   |
| Tayluan Santos  | Dev                  |
| Paulo Dante     | Tester               |
| Pamela Almeida  | Master               |
| Clara Araujo    | Dev                  |

## **3. DESCRIÇÃO**

- Criar a branch **task_06**, para trabalharmos as novas funcionalidades.
- Fazer um clone do repositório remoto para o local 
- Criar a pasta **auth** e, nela, suas subpastas, **entities**, **bcrypt**. Dentro da pasta **auth** criar o arquivo **auth.module.ts** (**Defina o módulo de autenticação**) e na pasta **entities** criar o arquivo **usuariologin.entity.ts**  (**Defina a entidade UsuarioLogin com suas propriedades**)

- Criar a Classe Bcrypt (**bcrypt.ts**). 

- Defina a classe Bcrypt com dois métodos: 

- Método **hashPassword**(password: string):
- Cria um hash criptografado da senha fornecida.
- Método **comparePassword**(password: string, hash: string):
- Compara a senha fornecida com um hash para verificar se elas coincidem.

Implemente o **AuthModule** e registre a classe **Bcrypt :**

- **providers**: Registra a classe **Bcrypt** para que possa ser usada e injetada dentro do **AuthModule**.
- **exports**: Torna a classe **Bcrypt** acessível para outros módulos que importam o **AuthModule**.

- Criar a pasta **usuario**. Dentro dela, crie as subpastas **bcrypt** e **entities**. Na pasta **entities**, crie o arquivo **usuario.entity.ts**. Em seguida, crie o arquivo **usuario.module.ts** na pasta **usuario**.

- **Criar o CRUD Completo do Recurso Usuário**

- Dentro da pasta **auth**, crie as subpastas (**guards**, **strategies**, **constants**, **services**)

- **Implementar o Passport com Estratégias Local e JWT**

- **LocalStrategy**: Para autenticação com nome de usuário e senha.
- **JwtStrategy**: Para validação de tokens JWT.
- **Configure os guards** e **módulo de autenticação** para usar essas estratégias.





## **4. Testes **

#### **CENÁRIOS POSITIVOS**

**Autenticar Usuário (Post): http://localhost:4000/usuario/login**

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXckzMUz-XjUJQUFH080t0TeiAbHkF3hrWER1ACIo_4f6bKBbX3aUhG8UCeVW8bqD4VB3rAJdxheXdrh0gYEOxnuO5ImP_Tu1YKhyjdPxFzlvnYbanKwALwKyQnxvP1zjKoJ7C5jwpMnvm9YtXPjj33l7oF6A_C87sY6OdI0SDz6qI_DGmCVgWI?key=My532E0ZvapoYVmLEG9Ovg)



**Atualizar Usuário (Put): http://localhost:4000/usuarios/atualizar**

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfu67-xNT5rU4MU8mGjovpLt8Oqe-m8Q2rx8lyIrRBNffW3YlENUIkSZdakrGsiJocBmKFGqGnzA0Nt9ZDxNAq3I8D6QcQG8mkb1v-c0_jE_lcqkzBHZY2FIbNz4ecNaRJ19Pfu8KveWVGnxwJLxHctGIbFgnVRY9qR-Tng47NUq9GMlUWNs88?key=My532E0ZvapoYVmLEG9Ovg)

**Listar todos os usuários (Get) : http://localhost:4000/usuarios/all**

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdXYHXnBl3M_RXKnRmzKpUkB5aDCuGfWaUZoU_lp5uM6oBUzqJQFoVIGukJiB678U-AXXr1e7Z-znqSPscLRboPIrcIgnAbsaZkcLILWspBgxkzbf0GnqfIb059Ja7xPwn9Pa1fKjAF7aFe7yAQedCXBUnQEQ8DB-4p2gx1n6xURuLs6kpCkww?key=My532E0ZvapoYVmLEG9Ovg)



#### **CENÁRIOS NEGATIVOS**

**Autorizar Usuário (Post) http://localhost:4000/usuarios/all**

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdwavF9aMq3Awg_haMj-TZdxUaOayfZBCgREuIc8-uXUVvx21TOm_j_I7EvLD1yM6VLyYH0rs1riCdjby4l8AgCZYAQeLPbbkFKZFq8t7r_eIUVztkIAn1W0SORjnAkvBYoTRrc580ktNErFSp0IsZc9UVzQkHHlvYtaLT49rYFwMA6nolSraA?key=My532E0ZvapoYVmLEG9Ovg)

**Listar Usuários por ID (Get) : http://localhost:4000/usuarios/1**

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcO55mmnfGtzZpuSZXlKCo9P3Uh8ghsV74Ruu1jt-TAS8zfMapIW1yqyw02FeOybwCBPafWePMAlEzq594Z67W37NkjodgAxlIWKCJQLCGkgdD4KXgkVbNR7McM0cCYk8mLsDR-LLZqWD_U__5OBIr8V9zSln5hAkvCSIG-YmYMri9_fV-IpxU?key=My532E0ZvapoYVmLEG9Ovg)

**Criar Produto (Post): http://localhost:4000/Produtos**

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdHrThdcblP99w9HX31h__Zxh8JY3cTA_P6Vsag6p_aOTEhlzU9A_9Jpc1Frk6hmhqaD1zxo3-ZeLrcqDV-142dV_3Znv85LlSz8vkZJU6lqC0WJwlVINdYRcWhDsB6SscWwbHTtb6RXgt0DwTyGiDzaB1ui-YhmreQbOQDq5jjBntCoeLfnEs?key=My532E0ZvapoYVmLEG9Ovg)

**Apagar Produto (DELETE): http://localhost:4000/Produtos/1**

![img](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc2Mpo9GJzzMTHHaZ5h2oQeX4r8AGw9vn8m2lZ23f6LuibXkbNqD-cA3ebiGuFqT3ZVnwKqS5iKmnA8nXgvjdlR9COdl007Onxxnu3SLAzP68DyPiPwKnYIMlZmmgqG7pDUwUx9QqH24k4jPfxwrGUsmbg4pemEimSh35Qjr-ZfIaIShre0cmM?key=My532E0ZvapoYVmLEG9Ovg)

## **5 - LINK DO REPOSITÓRIO**

https://github.com/Projeto-Vital 

