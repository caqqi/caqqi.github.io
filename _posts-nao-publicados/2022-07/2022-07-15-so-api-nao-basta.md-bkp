---
layout: post
title:  "Só a api não basta, falta criatividade"
author: bruno
categories: [ Java, Spring Boot ]
tags: [springboot, junior, jr, java]
image: assets/images/11.jpg
description: "Conteúdo só para ~~baixinhos~~ juninhos"
featured: false
---


## Conteúdo só para ~~baixinhos~~ juninhos

Quando estamos programando, eu acredito que seja:

- 30% - Leitura
- 20% - Escrita
- 50% - Pensamento / Análise / **Criatividade**

(esses números podem mudar dependendo de cada caso, pessoa ou mesmo não fazer sentido)

É comum vermos posts do pessoal que está começando ou que fez o ultimo Bootcamp da moda mostrando que conseguiu fazer uma API REST com Java e Spring Boot que por sua vez está gravando os dados no banco de dados.

Isso é legal. Mostra que estamos "pegando as coisas" bem rápido, mas se pararmos para análisar, está faltando algo ai e é coisa muito importante.


### Autópisia de uma API

![walking]({{ site.baseurl }}/assets/images/posts/2022-07/imagem-api-controller.png)

É um ```Controller/RestController``` do dia-a-dia, algo até muito interessante para quem está começando no Spring/Spring Boot. Mas perceba, é uma **classe Java normal** com algumas anotações do Spring -- E se vc já está mexendo com Spring Boot: **Classes, Métodos, Atributos, Parametros, String, Integer, Objeto** deve ser algo **NORMAL** (Não queria mexer em framework caso você não esteja confortavél com isso)!

Voltando ao ```Controller``` perceba, **é um método com apenas uma linha**, não há logica aqui:

```java
@GetMapping
public ResponseEntity<List<Cliente>> listarClientes() {
    return ResponseEntity.ok(clienteService.listarClientes());
} 
```

Vamos análisar o ```Service``` agora:

![walking]({{ site.baseurl }}/assets/images/posts/2022-07/imagem-api-service.png)

Novamente **é um método com apenas uma linha**, não há logica aqui:

```java
public Cliente obterDadosCliente(Long clienteId) {
    return clienteRepository.findById(clienteId).orElse(null);
}
```

Vamos análisar o ```Repository``` agora:

![walking]({{ site.baseurl }}/assets/images/posts/2022-07/imagem-api-repository.png)

E novamente não há nada aqui, nem se quer o método de uma linha.

```java
@Repository
public interface ClienteRepository extends JpaRepository<Cliente, Long> { }
```

Sem mais delongas, falta **criatividade**. 
Usamos apenas o framework com tudo que ele nos fornece e ja vem pronto. Não há **lógica** envolvida 
só chamadas de métodos que por sua vez tem apenas uma linha chamando outro método. 
Não colocamos nada de novo, não há uma coisa inventada por mim (eu como programador que estou programando o projeto). 

Faltou ```if's, whiles, for's```, outras classes que eu mesmo invento. 
Uma lógica totalmente aleatória que eu criei, algo que de um toque de criatividade, 
que mostre que estou indo além de usar o framework (e o que já vem pronto) e criar coisas, me desafiar.
Lembre-se: No mundo real o "buraco é mais embaixo".

Quando você entrar no mercado de trabalho para construir ou dar manutenção em sistemas 
você não fara só: **chamadas de métodos que por sua vez tem apenas uma linha chamando outro método**. Irão existir 
as **Regras de Negócios** - ideias (que devem ser transformadas em código) da mais pura criatividade possivél. 
E você terá que fazer isso, terá que entender o que outra pessoa pensou/criou e transformar em código apartir disso. 
Dai vão surgir ```if's, whiles, for's, classes, métodos, chamadas para outros sistemas``` 
e novamente (sendo repetitivo): **não será apenas métodos com uma linha chamando outro método**

### OK, entendi e como eu faço agora
Vamos refazer esse CRUD/API igualzinho como foi comentado aqui. Só que de um ponto em diante, será tudo por nossa conta. Tudo será criado da nossa cabeça, enfrentando um desafio de cada vez. Eu espero que você perceba o momento onde "**terminamos o básico e aprtir dai adicionamos funcionalidades novas criadas a partir do zero, usando puramente nossa criatividade**". Esse momento é muito importante. É onde estamos realmente aprendendo, descobrindo, desbravando o novo e fixando o conteúdo passado.

Vou usar coisas legais como:

> - Spring Boot
> - JUnit 5 para os testes unitários
> - Consumo de uma api externa
> - Leitura de arquivo
> - Banco de dados e etc

Bom, eu acredito que será muita coisa para ser escrita então eu vou fazer isso através de video/live coding e se gostou e quiser acompanhar, segue o link (abaixo) para a playlist onde desenvolvi uma api que chamei de **Descontão** e coloquei toda criatividade possivél.

[[ * LINK AQUI * ]]

Te velo lá,
{}'s
