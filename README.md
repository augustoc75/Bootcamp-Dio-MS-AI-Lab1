# Bootcamp-Dio-MS-AI-Lab1
Arquivos do projeto "Trabalhando com Machine Learning na Prática no Azure ML"

1. No portal Azure criei um "Resource Group" para os projetos do Bootcamp DIO/MS de AI Fundamentals
2. Criei um recurso do tipo Azure Machine Learning no Resource Group criado na etapa anterior
3. Após o deployment do recurso criado no passo 2, iniciei o Azure Machine Learning Studio
4. No Azure ML Studio, criei uma tarefa do tipo regressão por meio da opção "Automated ML"
5. Criei uma fonte de dados usando um arquivo .csv contendo dados históricos de locação de bicicletas
6. Ajustei os parâmetros conforme recomendações contidas no roteiro do ms-learn
7. Submeti o job
8. Alguns minutos depois o job rodou completamente e indicou o melhor modelo
9. Continuando as instruções do roteiro, fiz o deploy do modelo que apresentou o melhor resultado
10. O deploy falhou com a mensagem de erro: "ResourceOperationFailure: Resource provider [N/A] isn't registered with Subscription [N/A]."
11. Pesquisando na base de conhecimento da Microsoft, apliquei a solução recomendada que consistia em registrar dois provedores de recursos na minha assinatura do Azure, a saber: Microsoft.Cdn e Microsoft.PolicyInsights (https://learn.microsoft.com/en-us/answers/questions/2129910/resource-provider-(n-a)-isnt-registered-with-subsc) 
12. Após registrar os provedores de recursos, o deploy foi concluído com sucesso
13. 
