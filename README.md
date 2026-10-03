# Ecommerce Checkout - Testes Unitários com xUnit

Projeto desenvolvido para a disciplina de Gestão e Qualidade de Software.

O objetivo deste projeto é implementar funcionalidades básicas de um checkout de e-commerce utilizando C# e .NET 10, aplicando testes unitários com xUnit.

## Funcionalidades

A classe `PedidoService` possui os seguintes métodos:

### GerarCodigoRastreio

Gera um código de rastreio utilizando a região em letras maiúsculas e o número do pedido com 4 dígitos.

Exemplo:

```text
sudeste + 42 = SUDESTE-0042
```

### CalcularPontosFidelidade

Calcula os pontos de fidelidade do cliente.

A cada R$ 10 em compras, o cliente recebe 2 pontos.

Exemplo:

```text
R$ 150 = 30 pontos
```

### TemDireitoAFreteGratis

Verifica se o cliente possui direito a frete grátis.

O frete será grátis quando:

- O valor da compra for maior ou igual a R$ 200;
- Ou o cliente for VIP.

## Testes Unitários

Os testes foram desenvolvidos utilizando xUnit.

Foram implementados 4 testes:

- Validação da geração do código de rastreio com `Assert.Equal`;
- Validação do cálculo de pontos de fidelidade com `Assert.Equal`;
- Validação de frete grátis para cliente VIP com `Assert.True`;
- Validação de frete para cliente não-VIP com `Assert.False`.

## Executando os testes

Para executar os testes, abra o terminal na pasta do projeto e utilize:

```bash
dotnet test
```

Resultado esperado:

```text
total: 4
falhou: 0
bem-sucedido: 4
```

## Tecnologias utilizadas

- C#
- .NET 10
- xUnit
- Git
- GitHub

## Autor

Gabriel Gobira de Souza