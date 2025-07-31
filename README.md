# pipeline-mlops-aws
Deploy  do  modelo  de  Machine  Learning através de API em nuvem AWS

Estes scripts vão servir apenas como base para apoiar a configuração AWS

![Solução](/images/overview.png)


- Criar o buket "pinguins-890582101704" e carregar o dataset.csv
- Abrir o Sagemaker studio e carregar o script .ipynb no Jupyter lab e executar os scripts para salvar o modelo no S3
- Configurar a politica de acesso criando um perfil com os acessos:
    - AWSLambdaBasicExecutionRole
    - AmazonSageMakerFullAccess
- Criar a função Lambda com o codigo do script lambda_function.py
- Criar REST API com API Gateway e no método configurar o POST para a função Lambda

![Teste Lambda](/images/teste_lambda%20.png)

### Obs: Ainda quero automatizar isto tudo com IAC 
