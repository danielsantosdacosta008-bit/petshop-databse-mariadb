# petshop-databse-mariadb
Modelagem e consultas SQL para sistema de pet shop hospitalar.


1.1 CREATE DATABASE PETSHOP

<img width="764" height="327" alt="image" src="https://github.com/user-attachments/assets/ed59b178-7301-42ea-9334-e4c89884e8b9" />


1.2 USE DATABASE PETSHOP

<img width="550" height="155" alt="image" src="https://github.com/user-attachments/assets/3be3ae43-d439-427a-8e42-92667560813b" />

2. CREATE TABLES

1.1	Create table clientes
 
<img width="1048" height="53" alt="image" src="https://github.com/user-attachments/assets/05c6f2ac-1c7d-4419-83af-d94a5814316c" />


1.2	Create table veterinários
 
<img width="1042" height="61" alt="image" src="https://github.com/user-attachments/assets/f9636bf1-a172-41e4-a46f-4f07e0911193" />


1.3	Create table pets
 
<img width="886" height="48" alt="image" src="https://github.com/user-attachments/assets/002da2ac-4122-408e-bafe-615be4a05e83" />


1.4	create table medicamentos_procedimentos

<img width="995" height="134" alt="image" src="https://github.com/user-attachments/assets/e739adc2-98ef-49c5-a76f-4ed07ba5152a" />


1.5	Create table consulta

<img width="1031" height="89" alt="image" src="https://github.com/user-attachments/assets/eff92ee8-600e-44df-ac2e-5a68033f0e32" />

 
1.6	Create table prSecricao

<img width="886" height="661" alt="image" src="https://github.com/user-attachments/assets/6ec682d6-9705-43e1-9761-0a665f668924" />

2.ADD REGISTROS

2.1 Add registros clientes

<img width="886" height="489" alt="image" src="https://github.com/user-attachments/assets/ac2d515b-1365-44ef-bcbe-c153577a14d9" />
<img width="886" height="825" alt="image" src="https://github.com/user-attachments/assets/a826095b-5dc7-4f0b-8e7a-bbc9aa72f50e" />

 
2.2 Add registros pets

<img width="886" height="371" alt="image" src="https://github.com/user-attachments/assets/feb7d47e-d10c-4ee5-80ec-5b2821d0322d" />
<img width="886" height="359" alt="image" src="https://github.com/user-attachments/assets/f08ecc15-aaf4-4cb1-916a-9af155a3d96a" />

 
2.3 Add registros veterinários

<img width="867" height="512" alt="image" src="https://github.com/user-attachments/assets/7fce7310-37fb-43c1-99e3-3961276e04bd" />

 
2.4 Add registros Medicamentos_procedimentos

<img width="886" height="600" alt="image" src="https://github.com/user-attachments/assets/73be955f-a1e7-450c-bf08-0a40da72195a" />
<img width="886" height="496" alt="image" src="https://github.com/user-attachments/assets/fac1b8a9-2986-4198-924e-210b36b46d31" />

 
2.5 Add registros consulta

<img width="886" height="256" alt="image" src="https://github.com/user-attachments/assets/d65e715f-a803-4079-b65f-3f3d566ca7f9" />
<img width="886" height="623" alt="image" src="https://github.com/user-attachments/assets/c718f678-b6e0-4cd5-947b-ad24fb619da4" />

 
2.6 Add registros prescrição

<img width="886" height="270" alt="image" src="https://github.com/user-attachments/assets/b134fe8e-0d62-4328-963b-e6c72a10537b" />
<img width="663" height="433" alt="image" src="https://github.com/user-attachments/assets/15de1afc-1de2-4951-8253-2e3c5f7e75e4" />

3. UTILIZANDO CONSULTA SQL
   
3.1 Select

<img width="886" height="255" alt="image" src="https://github.com/user-attachments/assets/4feae627-dc6a-4412-a719-0911c9761c0b" />

 
3.2 Where

<img width="733" height="441" alt="image" src="https://github.com/user-attachments/assets/b56d5489-f281-4cb2-8791-bc1f0dacee6a" />

 
3.3 Order by
Nome

<img width="886" height="425" alt="image" src="https://github.com/user-attachments/assets/36fea6ab-db77-40de-b93d-7648f0edab72" />

Nascimento

<img width="886" height="165" alt="image" src="https://github.com/user-attachments/assets/f5ef2daf-9d06-485a-8e44-59f3d152d226" />

3.4 Like

<img width="886" height="195" alt="image" src="https://github.com/user-attachments/assets/a62dace6-77ab-4207-91cd-be548dcad538" />

 
3.5 Between

<img width="886" height="213" alt="image" src="https://github.com/user-attachments/assets/cb57db93-d707-49d2-b110-c14ed58cabaf" />

 
3.6 In

<img width="694" height="663" alt="image" src="https://github.com/user-attachments/assets/591a3862-21aa-4359-ab45-697f6378a4c0" />

4. JOIN

4.1 Inner Join

#Lista dados dos pets e seus respectivos donos. -- Só mostra registros que possuem vínculo ativo nas duas tabelas (Pet + Dono)

<img width="886" height="425" alt="image" src="https://github.com/user-attachments/assets/8e7fe498-ef45-4dc6-b6c4-0e1c36fb36ef" />

 
#Monta o histórico clínico completo das consultas. -- Junta 3 tabelas para trocar os códigos de ID pelos nomes reais do pet e do médico.
 
<img width="634" height="641" alt="image" src="https://github.com/user-attachments/assets/445b6a03-54fc-4848-8cc0-346a86a67786" />


4.2 Left Join

#Lista TODOS os clientes, mesmo aqueles que não têm nenhum pet. -- Garante que o cliente apareça na lista; se não tiver pet, o campo do animal vem como NULL.

<img width="886" height="276" alt="image" src="https://github.com/user-attachments/assets/6c026fa2-3903-424d-8add-3ba20b34abe5" />

 
#Filtra para encontrar medicamentos ou exames nunca utilizados. -- Traz tudo da tabela clínica e o 'is null' isola o que ficou sem vínculo na prescrição.

<img width="845" height="350" alt="image" src="https://github.com/user-attachments/assets/5f382e7b-4866-4a22-b61f-4ce3c56302ff" />

5. ALTER TABLE

5.1 Adicionar coluna

#Adicionando email
<img width="886" height="374" alt="image" src="https://github.com/user-attachments/assets/ed546c76-0b5a-413f-96dd-7bbaf1e7d387" />

5.2Modify

#Modificando limite varchar email
<img width="886" height="355" alt="image" src="https://github.com/user-attachments/assets/f9f22c98-3e5f-4e53-96d6-aa3f5b1155ad" />

5.3 Change

#Alterando nome

<img width="886" height="359" alt="image" src="https://github.com/user-attachments/assets/2f84be7f-b3ff-42e5-b33d-220835436d0a" />

 
5.4 Drop

#Deletando coluna

<img width="669" height="402" alt="image" src="https://github.com/user-attachments/assets/9c61659a-1948-4391-83f0-544fcf335697" />

 
6. UPDATE e DELETE

6.1

#Atualizar registros

<img width="886" height="517" alt="image" src="https://github.com/user-attachments/assets/bd8bcb68-7b6d-45e8-b200-835e3c7793a5" />

 
#Excluir registros

#Antes de excluir o id=14

<img width="659" height="389" alt="image" src="https://github.com/user-attachments/assets/e2316294-062c-4f9b-b23d-73075ad6aa54" />

 
#Depois de excluir o id=14

<img width="886" height="64" alt="image" src="https://github.com/user-attachments/assets/e99df8c4-5b94-4498-a993-95c79040e9ea" />

 
7. JSON

7.1 Insert com JSON

<img width="886" height="301" alt="image" src="https://github.com/user-attachments/assets/1d6d0876-b044-4864-863c-d12dfd535c53" />
![Uploading image.png…]()

 
