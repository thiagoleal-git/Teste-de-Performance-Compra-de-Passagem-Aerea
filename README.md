Aqui está o README atualizado com a informação solicitada:

# Teste de Performance - Compra de Passagem Aérea

## Introdução

Este documento descreve o teste de performance realizado para simular a compra de uma passagem aérea no site https://www.blazedemo.com.

Critério de Aceitação:
* 250 requisições por segundo com um tempo de resposta 90th percentil inferior a 2 segundos.

## Ferramenta Utilizada

O teste de performance foi desenvolvido utilizando a ferramenta JMeter.

## Configuração e Execução do Teste

O teste foi configurado para simular a compra de uma passagem aérea com sucesso. Foram utilizados 250 usuários virtuais (threads) para atingir a vazão desejada (250 requisições por segundo).

O teste foi iniciado às 17:45:23.354 e finalizado às 17:45:23.852, com um tempo total de execução de 46.988 segundos.

## Resultados

Durante o teste, a aplicação atingiu uma vazão de 250 requisições por segundo. No entanto, apenas 122 das 250 requisições tiveram um tempo de resposta inferior a 2 segundos e não houve falhas.

## Conclusão

O critério de aceitação não foi atingido porque o tempo de resposta do 90º percentil foi superior a 2 segundos. Além disso, houve uma falha em uma das requisições.

Possíveis causas para o tempo de resposta alto e a falha na requisição incluem:
- Problemas de desempenho no lado do servidor, como falta de recursos (CPU, memória, largura de banda), gargalos no banco de dados ou problemas de configuração.
- Problemas de desempenho no lado do cliente, como falta de recursos ou problemas de rede.
- Problemas com o próprio teste, como a seleção de ferramentas inadequadas, falta de uma estratégia de teste adequada ou cobertura insuficiente do teste.

Sugestões para melhorar a performance e evitar falhas nas requisições incluem:
- Identificar e corrigir problemas de desempenho no lado do servidor, como otimizar consultas ao banco de dados, aumentar os recursos disponíveis ou ajustar as configurações do servidor.
- Identificar e corrigir problemas de desempenho no lado do cliente, como otimizar o código do aplicativo ou melhorar a conectividade de rede.
- Revisar e aprimorar o plano de teste, selecionando as ferramentas adequadas, desenvolvendo uma estratégia de teste abrangente e garantindo uma cobertura adequada do teste.

## Instruções para Execução do Script

Para executar o script, siga os seguintes passos:

1. Instale o JMeter na sua máquina.
2. Clone este repositório: git@github.com:thiagoleal-git/Teste-de-Performance-Compra-de-Passagem-Aerea.git
3. Abra o script "Teste de Compra de Passagem Aérea" no JMeter.
4. Execute o script.
5. Os resultados serão gerados em um arquivo .jtl na mesma pasta onde o script do teste está localizado.

## Relatório de Execução dos Testes

Devido a problemas não identificados no ambiente ou setup, não foi possível gerar o relatório do resultado em HTML. O relatório pode ser encontrado na pasta Relatórios Jmeter dentro da pasta bin.
