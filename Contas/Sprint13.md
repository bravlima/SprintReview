# Sprint 13

## Contas com KYC rejeitado
Foi testado o incidente identificado em relação a criação de contas quando o KYC é inválidado e posteriormente o mesmo passa a ser validado.

#### Status inicial
![StatusConta](./arquivos/KYC/1_Status_Conta.png)

#### Status KYC rejeitado
![StatusRejeitado](./arquivos/KYC/3_Status_KYC_Rejeitado.png)

#### Status KYC aprovado
![StatusAprovado](./arquivos/KYC/5_Status_KYC_Aprovado.png)

## Botão 'Validar' criação de chave PIX
Foi concluído os testes em relação ao botão 'Validar' disponivel no processo de criação de chave quando esse não é concluído.

![Validar](./arquivos/validar.jpg)

![Validado](./arquivos/validado.jpg)

## Ícones incorretos
Foi realizado teste em relação aos icones das transações que não estavam sendo apresentadas.</br>
Porém, conforme avaliado em refinamento, esta situação pode ser decorrente de cache onde cabe uma Spike para uma melhor avaliação.

![Pix](./arquivos/Screenshot_27.png)

![Transferência](./arquivos/Screenshot_28.png)

## Criação de contas com erro na Pismo
Teste realizado a partir de uma ocorrência onde foi observado que não está sendo criado conta devidamente apresentando o erro 'Linked_Pismo_Celcoin_Error'.</br>
Foi realizado teste em ambiente de QA para garantir que a criação de contas se manteve sem falhas.

## Descrição da opção 'Receba com um QRcode'
Foi concluído o teste em relação a correção do texto para recebimento de valores via QRcode, onde estava pendente a validação no iOS.

![MeuEscritório](./arquivos/meuEscritorio.jpg)

![MeuNegocio](./arquivos/meuNegocio.jpg)

## Garantir que o app iOS esta abrindo
Tivemos um problema em uma das builds que quebrou o app no iOS impossibilitando a abertura do mesmo, onde a situação foi corrigida e o app está ok, conforme pode ser visto pelas imagens dos demais testes feitos no iOS.