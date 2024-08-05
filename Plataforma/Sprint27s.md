# Sprint 27s

## Party Service
### Adaptar CreatePersonCredentialUseCase
Foi testada a implementação que visa alterar a criação de person, permitindo que sua senha seja atualizada.

*Ref*.: [US_661310](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/661310)

### Permitir alterar metadata da entidade Person
Teste da implementação que passou a permitir alterar o metadata da entidade person

*Ref*.: [US_663942](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/663942)

### Salvar metadata da entidade Organization
Teste da implementação que passou a permitir salvar o metadata da entidade organization

*Ref*.: [US_663090](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/663090)

## IBK
### Alteração URL do IBK Transition
Testada a alteração que alterou a URL do IBK transition.

*Ref*.: [US_648338](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/648338)

### Login IBK Transition
Foi realizado teste na implementação que visa adequar o login do IBK Transition.</br>
Essa US resultou em alguns levantamentos de melhoria/adequação, devido a limitações observadas no BE e FE, os pontos estão devidamente documentado na US.

*Ref*.: [US_665505](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/665505)

### Seleção de empresas IBK Transition
Teste da implementação que passou a permitir realizar a seleção de empresas no IBK Transition

*Ref*.: [US_634249](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/634249)

### Redirecionamento para Home
Teste da implementação que ajustou o redirecionamento para a home após a seleção de empresas no IBK Transition

*Ref*.: [US_663960](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/663960)

## Migration Service
### Reutilizar entidade person já existente
Teste parcial da implementação que visa reutilizar a entidade person já existente na migração de contas.</br>
Trata-se de um teste parcial, pois para testar o cenário completo seria preciso que o Migration Service já estivesse totalmente implementado considerando o cenário de uma mesmo person possuir mais de uma conta.</br>
Este fluxo será testado em sua completude em outra US especifica.

*Ref*.: [US_663088](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/663088)

### Parametrizar reversão para não alterar Keycloak
Teste da implementação que passou a permitir não reveter as alterações de Keycloak e Credenciais, ao reverter a migração de uma conta.

*Ref*.: [US_663087](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/663087)

## SuperApp
### Lista de empresas com conta digital ao logar
Validada a implementação que tinha como objetivo passar a listar as empresas com conta digital.</br>
Durante o desenvolvimento, foi observado também a existência de uma limitação do BE na listagem destes dados, sendo necessário uma adequação e por este motivo, foi reportado a necessidade de reteste após conclusão da implementação do BE para garantir que está sendo listado também organizações sem conta bancária.

*Ref*.: [US_659002](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/659002)

### Primeiro login no device
US de test only que tinha como finalidade testar e validar a implementação de autenticação de device via SMS ou E-mail em um primeiro acesso em novo device.

*Ref*.: [US_604751](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/604751)

## BFF Meu Escritório
### Aceitar parametro PartyId endpoint party-service has-credentials
Teste da implementação que visa a utilização do parâmetro PartyID para consultar a existstência de credenciais de acesso.

*Ref*.: [US_661964](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/661964)

### Ajuste endpoint listagem de empresas e contas bancárias
Foi realizado teste quanto ao ajuste no endpoint de listagem de empresas e contas bancárias visando listar todas as empresas mesmo sem contas bancárias.

*Ref*.: [US_667056](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/667056)