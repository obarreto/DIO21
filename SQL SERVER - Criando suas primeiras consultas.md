```sql
CREATE TABLE Teste 
{
	Descricao varchar(50) null,
	Complemento char(10) NOT null
}

INSERT Teste VALUE(null, 'b')
```

```sql
CREATE TABLE Produtos
{
	Codigo int,
	Nome varchar(100),
	Descricao varchar(200),
	Preco float
}

```

```sql
CREATE TABLE Clientes
{
	Codigo int,
	Nome varchar(100),
	TipoPessoa char(200)
}
```

```sql
CREATE TABLE Pedido
{
	Codigo int NOT null,
	DataSolitacao datetime,
	FlagPago bit NOT null,
	TotalPedido float NOT null,
	CodigoCliente int NOT null
}
```

```sql
CREATE TABLE PedidoItem
{
	CodigoPedido int NOT null,
	CodigoProduto int NOT null,
	Preco float NOT null,
	Quantidade int NOT null
}
```

```sql
SELECT * FROM clientes

INSERT INTO Clientes (codigo, nome, TipoPessoa) VALUES (1, 'Thiago', 'F')
INSERT Cliente (codigo, nome, TipoPessoa) VALUES (2, 'Thiago', 'F')
INSERT clientes VALUES ('4', 'Thiago', 'I')
INSERT clientes ('5', 'Thiago', 'F'), (1, 'Thiago', 'J')

SELECT * 
FROM clientes 
WHERE TipoPesso = 'J'
```

```sql
UPDATE cliente 
SET    Codigo = 7,
	   Nome = 'Jose'
WHERE TipoPesso = 'J'
```

```sql
DELETE 
FROM cliente
WHERE codigo in (5, 4, 3, 2)
```



```sql
INSERT Produtos VALUES(1, 'Caneca', 'Caneca Azul', 1.5)
INSERT Produtos VALUES(2, 'Caderno', 'Caderno 10 mat', 20.99)
```

```sql
--
INSERT Pedido VALUES (1, getdate(), 0, 3, 7)

INSERT Pedido VALUES (1, 1, 1.5, 2)

INSERT Pedido VALUES (1, 1, 22.49, 2)
```

```sql
SELECT isnull(dataCricao, getdate(), * FROM clientes
```

```sql
SELECT *, 
		CASE 
			WHEN TipoPessoa = 'J' THEN 'Juridica'
			WHEN TipoPessoa = 'F' THEN 'Fisica'
			ELSE 'Pessoa indefinida'
			end = GETDATE() -- erro
FROM 		clientes
```

```sql
SELECT *, CONVERT(VARCHAR (50), DataSolicitacao, 103)
FROM Pedido

```

```SQL
SELECT *, 
		CASE 
			WHEN TipoPessoa = 'J' THEN 'Juridica'
			WHEN TipoPessoa = 'F' THEN 'Fisica'
			ELSE 'Pessoa indefinida'
			end = CONVERT(VARCHAR, GETDATE(), 105)
FROM 		clientes
```

