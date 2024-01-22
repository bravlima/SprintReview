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
#### Chave à validar
![Validar](./arquivos/validar.jpg)

#### Chave validada
![Validado](./arquivos/validado.jpg)

## Ícones incorretos
Foi realizado teste em relação aos icones das transações que não estavam sendo apresentadas.</br>
Porém, conforme avaliado em refinamento, esta situação pode ser decorrente de cache onde cabe uma Spike para uma melhor avaliação.
#### Ícone do PIX
![Pix](./arquivos/Screenshot_27.png)

#### Ícone de Transferência
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

## Ocultação botão 'Exportar Extrato'
Validação da implementação que visava esconder o botão 'Exportar Extrato' do IBK.</br>
Essa alteração foi implementada corretamente, porém, poderá ser apresentada ainda a depender do acesso, devido ao cache.

![ExportarExtrato](./arquivos/exportarExtrato.png)

## Correção número telefone perfil do usuário IBK
A correção em questão visava ajustar a apresentação do telefone no perfil do usuário, onde devido o código +55 estava fazendo com que o número fosse apresentado de forma incorreta.

![TelContato](./arquivos/telContato.png)

## Criação de conta para contas já existentes na Pismo
Testado a criação de contas para contas já existentes na Pismo, onde estava ocorrendo erro ao criar uma nova conta quando essa já existia na Pismo.

![ContaBackoffice](./arquivos/contasBackoffice.png)

## Limite de caracteres para nome da empresa
Testada a implementação que visa limitar a quantidade de caracteres para o nome da emrpesa na criação da conta na Pismo, onde deverá ser considerado o limite de 60 caracteres.

![NamePismo](./arquivos/namePismo.png)

![CompanyName](./arquivos/companyPismo.png)

## Gravar eventos no banco de dados
Foi testado a implementação/correção da US que visava implementar a gravação dos dados de emissão/pagamento de boletos do bankslip.
#### Emissão de Boleto
![EmissãoBoleto](./arquivos/emissaoBoletoBanco.png)

#### Pagamernto de boleto
![PagamentoBoleto](./arquivos/pagamentoBoletoBanco.png)

## Tela de login indevida
Os app apresentavam a tela de login com loading infinito em algumas situações, como no fluxo P2P, Pagamento de Contas.

Essa US gerou retorno, pois foi possível gerar a tela de login em outras situações.

## Internal Server na transferência PIX
Ao realizar uma transferência PIX estava sendo realizada uma requisição para o endpoint pix-transfer-return-reasons que retornava 500, porém, se tratava de uma requisição indevida neste momento.

![InternalErrorPix](./arquivos/pix500.gif)

## Correção do campo Nickname
Ao confirmar os dados para transferência PIX estava sendo apresentado o campo 'Nickname', sendo o correto apresentar 'Apelido do Contato'.

![Nickname](./arquivos/nickname.png)

## Bloqueio de pagamento de guia iniciada em 81/85 IBK
Foi reimplementado o bloqueio no FE para impedir o pagamento de guias de impostos iniciados em 81/85
#### Guia iniciada em 81
![Guia81](./arquivos/guia81.png)

#### Guia iniciada em 85
![Guia85](./arquivos/guia85.png)

### Bloqueio de pagamento de guia iniciada em 81/85 App
Também foi realizada a mesma implementação nos app's
#### Guia iniciada em 81 - iOS
![Pagto81ios](./arquivos/pagto81ios.jpg)

#### Guia iniciada em 85 - iOS
![Pagto85ios](./arquivos/pagto85ios.jpg)

#### Guia iniciada em 81 - Android
![Pagto81android](./arquivos/pagto81android.png)

#### Guia iniciada em 85 - Android
![Pagto85android](./arquivos/pagto85android.png)

## Descrição das trasferências P2P no IBK
Foi realizado testes em relação ao tratamento da descrição da movimentação de transferências P2P no IBK para que fossem apresentadas como 'Transferência enviada' e 'Transferência recebida'.
#### Transferência enviada
![TransfEnviada](./arquivos/transfEnviada.png)

#### Transferência recebida
![TransfRecebida](./arquivos/transfRecebida.png)

## Comprovante PIX no IBK
Validada a correção do comprovante PIX no IBK onde ao concluir a transação, não estava trazendo os dados corretamente.</br>
A situação ocorria também ao clicar em 'Compartilhar'.
#### Comprovante ao concluir transação
![ComprovantePosOperacao](./arquivos/comprovantePosOperacao.png)

#### Comprovante ao clicar em 'Compartilhar'
![ComprovanteCompartilhar](./arquivos/comprovanteCompartilhar.png)

## Ociosidade/Demora na transferência P2P
Ao realizar uma transferência P2P cadastrando um novo favorecido o sistema apresentava uma ociosidade/demora no processo de cadastro do favorecido e ao concluir a transferência, os dados no comprovante não eram gerados corretamente.
#### Android
![TransfP2P](./arquivos/transfCNPJ.gif)

#### iOS
![Comprovante](./arquivos/comprovante.JPG)

## Opções ocultas no cadastro de favorecido
Os campos de 'Conta' e 'Digito' não deverão estar visiveis ao usuário no cadastro de favorecidos.

![CadastroFavorecido](./arquivos/cadastroFavorecido.png)

## Descrição recebimento P2P
Teste em relação a descrição do recebimento P2P onde trazia indevidamente a descrição 'Você pagou'.
#### iOS
![RecebimentoiOS](./arquivos/recebimentoP2P.jpg)

#### Android
![RecebimentoAndroid](./arquivos/Screenshot-2024-01-20T14-18-21.375Z.png)

## Tela de login com loading infinito
Durante a sprint foi tratado a tela de login com loading infinito, o qual gerou também um bug para esta mesma situação, porém a partir de uma origem distinta.</br>
Ambas as situações não foram mais reproduzidas em novos testes.