# Desafio2BootcampAWSCodeGirls
Desafio 2 do Bootcamp, referente aos fluxos AWS Step Functions
**AWS Step Functions - Exemplo do fluxo de trabalho**

Trata-se do desafio 2 referente ao Bootcamp Code Girls do Santander, em parceria com a DIO, originado no módulo que trata de AWS Step Functions.

**Descrição do Fluxo**

Gerei o fluxo descrito a seguir com o objetivo de simular um workflow de verificação de arquivos, após a verificação de “true” ou “false” após a entrada de arquivos.

A seguir, o detalhamento do fluxo:

1. **Start** - início do fluxo
2. Aviso do arquivo para uma fila SQS
3. **Verificação de arquivos -** task feita pelo Lambda
4. **Choice State**
    1. **Se true -** vai para o próximo passo de processamento de arquivos
    2. **Se false** - vai para end
5. **Processamento do arquivo** - Lambda que pega o arquivo e o processa
6. **Bucket de saída**  - resultado gravado em buxket
7. **End** - conclusão do fluxo

**Arquivos do repositório**

**Readme.md**: documentação

**Arquivo JSON**: gerado no site da AWS
Arquivo: 1; fluxo e 3; prints da tela de elaboração