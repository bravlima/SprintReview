# Sprint 20s

## Party Service
### Validação de CPF
Foi realizado teste em relação a implementação do endpoint que tem como finalidade realizar a validação do CPF de forma a garantir a existência do pré-cadastro. A respectiva implementação ocorreu nos três serviços Meu Escritório, Minha Empresa e Empregado.</br>
*Ref*.: [US_630738](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/630738)

![ValidaçãoCPF](./arquivos/Screenshot_21.png)

### Correção de validações no endpoint de Download de arquivo
Na sprint passada durante os testes no endpoint de download de arquivo foi identificado a necessidade de algumas melhorias em relação as validações de ID, o qual foram implementadas nesta sprint.</br>
*Ref*.: [US_630580](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/630580)

## Correções e Segurança
### Correção do Mock para conta de prod
Foi realizado a correção dos Mocks das contas de prod. A partir desta correção, o disparo de SMS/Email deixou de ocorrer, no entanto, conforme validado em conjunto ao Bruno Tavares e Roberto, os logins ocorreram corretamente.</br>
*Ref*.: [US_630979](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/630979)

### Correção de segurança Prototype Pollution
Essa correção impactava o keycloak que por sua vez poderia gerar erros nos logins, desta forma foi realizado testes de logins no IBK, Backoffice, APPs, bem como validado as informações geradas pelo token JWT.</br>
*Ref*.: [US_621933](https://dev.azure.com/tr-ggo/TR%20Fintech/_workitems/edit/621933)

![TokenJWT](./arquivos/validade_jwt.png)