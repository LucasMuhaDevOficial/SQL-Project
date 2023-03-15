CREATE TABLE clientes (
    id INT PRIMARY KEY,
    nome VARCHAR(50),
    idade INT,
    email VARCHAR(100),
    telefone VARCHAR(20)
);

INSERT INTO clientes (id, nome, idade, email, telefone)
VALUES (1, 'João Silva', 30, 'joao.silva@gmail.com', '(11) 9999-9999'),
       (2, 'Maria Santos', 25, 'maria.santos@hotmail.com', '(21) 8888-8888'),
       (3, 'Pedro Souza', 40, 'pedro.souza@yahoo.com', '(31) 7777-7777');

SELECT * FROM clientes;

SELECT nome, idade FROM clientes WHERE idade > 30;

UPDATE clientes SET email = 'joao.silva@outlook.com' WHERE id = 1;

DELETE FROM clientes WHERE idade < 25;
