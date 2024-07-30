# Sprint 27s

## Party Service
### Adaptar CreatePersonCredentialUseCase
Foi testada a implementação que visa alterar a criação de person, permitindo que sua senha seja atualizada.

*Ref*.: [US_661310](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/661310)

### Permitir alterar metadata da entidade Person
Teste da implementaçãou que passou a permitir alterar o metadata da entidade person

*Ref*.: [US_663942](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/663942)

## IBK
### Alteração URL do IBK Transition
Testada a alteração que alterou a URL do IBK transition.

*Ref*.: [US_648338](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/648338)

### Login IBK Transition
Foi realizado teste na implementação que visa adequar o login do IBK Transition.</br>
Essa US resultou em alguns levantamentos de melhoria/adequação, devido a limitações observadas no BE e FE, os pontos estão devidamente documentado na US.

*Ref*.: [US_665505](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/665505)

## Migration Service
### Reutilizar entidade person já existente
Teste parcial da implementação que visa reutilizar a entidade person já existente na migração de contas.</br>
Trata-se de um teste parcial, pois para testar o cenário completo seria preciso que o Migration Service já estivesse totalmente implementado considerando o cenário de uma mesmo person possuir mais de uma conta.</br>
Este fluxo será testado em sua completude em outra US especifica.

*Ref*.: [US_663088](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/663088)

## SuperApp
### Lista de empresas com conta digital ao logar
Validada a implementação que tinha como objetivo passar a listar as empresas com conta digital.</br>
Durante o desenvolvimento, foi observado também a existência de uma limitação do BE na listagem destes dados, sendo necessário uma adequação e por este motivo, foi reportado a necessidade de reteste após conclusão da implementação do BE para garantir que está sendo listado também organizações sem conta bancária.

*Ref*.: [US_659002](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/659002)