# **Teste Systock - DevOps**

Esse é um desafio técnico solicitado pela empresa Systock, o desafio consiste em enviar os dados do banco de dados consumo_a para o banco consumo_b.

## **Problemas encontrados**

No banco de dados **consumos_b** a coluna **"status"** estava com tamanho de apenas **1 caractere**, enquanto no banco de dados **consumos_a** são **10 caracteres**, e o segundo problema é na coluna **valor**, que estava diferente do banco de dados consumos_a que a coluna está com nome **valor_total**.

## Soluções encontradas

### 1º Solução

1: Alterar dados da coluna status de "Devolucao" para "D" e "Venda" para "V", para caber no tamanho apresentado.
2: Identificar "Valor_total" = "Valor" dentro do **PDI** para envio dos dados equivalentes para coluna correta do banco de dados.

<img src="/src/fluxo1.png" alt="Fluxograma_1">

### 2º Solução

1: Alterar o valor do tamanho da coluna status para 10 assim caberiam os valores.
2: Alterar o nome da coluna valor, para valor total.

<img src="/src/fluxo2.png" alt="Fluxograma_2">