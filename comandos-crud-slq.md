 # Comandos para operações CRUD no Banco de dados

 ## Resumo

 - C -> CREATE (inserir dados usando comando `INSERT`)

 - R -> READ (ler dados usando comando `SELECT`)

 - U -> UPDATE (atualizar dados usando comando `UPDATE`)

 - D -> DELETE (excluir dados usando comando `DELETE`)

 ## INSERT

 ```sql
 INSERT INTO fabricantes (nome) VALUES('Asus');

 INSERT INTO fabricantes (nome) VALUES('Dell');
 INSERT INTO fabricantes (nome) VALUES('Apple');

 INSERT INTO fabricantes (nome) VALUES('LG'),('Samsung'), ('Brastemp');

 INSERT INTO fabricantes (nome) VALUES('Positivo'), ('Microsoft');
 ```

 ### Produtos

 ```sql
 INSERT INTO produtos(
    nome, preco, descricao, quantidade, fabricante_id)
    VALUES(
        'Ultrabook',
        3500,
        'Equipamento de ultima geração cheio de recursos com processador Intel Core i9 do balacobaco.',
        7,
        2 -- id do fabricante DELL
    );

    INSERT INTO produtos(
        nome, descricao, preco, quantidade, fabricante_id
    )
    VALUE(
        'Tablet Android',
        'Tablet com a versão 14 do sistema operacional Android,
         possui tela de 10 polegadas e armazenamento de 128 GB,
         e 64 GB de RAM porque o Eliel perguntou',
         1499.99,
         5,
         5
    );
 ```