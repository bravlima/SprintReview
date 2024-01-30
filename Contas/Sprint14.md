# Sprint 14

## Falha ao postar mensagem é tratado como lido
Foi testado a correção de uma falha que possuímos onde em casos onde ocorria erro na leitura da mensagem postada no webhook o sistema tratava como lido indevidamente.</br>
Com a correção, o step somente é atualizado após a leitura efetiva da mensagem.

#### Erro no KYC
![KYC500](./arquivos/KYC500.png)

#### Step sem atualização
![StepSemAtualizar](./arquivos/AccountStep.png)

#### Conta criada
![AccountCreate](./arquivos/AccountCreate.png)

## Envio do quadro societário para o Onvio
Teste realizado quanto a implementação que trata o envio do quadro societário na ausência do campo 'nationalIdentity'.</br>
Vale ressaltar que esta situação só foi reproduzida manipulando o JSON, visto que mesmo o campo não havendo informação o sistema envia uma string vazia e o erro ocorre apenas na ausência do campo.</br>

#### Erro no Agente
![ErroAgente](./arquivos/falhaAgente.png)

#### Reenvio da informação
![ReenvioQuadro](./arquivos/Quadro200.png)