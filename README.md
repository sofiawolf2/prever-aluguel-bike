
# Previsão Azure Machine Learning :bicyclist:

A partir de um desafio da DIO, criei esse modelo de previsão de aluguel de bicicletas com endpoints (pontos de extremidade) ja configurados. Aqui irei mostrar o passo a passo de minha jornada.
### Material de apoio:

Alem das aulas sobre o assunto, usei como material de apoio o link [Explore Automated Machine Learning in Azure ML](https://microsoftlearning.github.io/AI-900-AIFundamentals/instructions/02-module-02.html#clean-up).

## Descrição em etapas

|nº  | Etapas|
|-----:|-----------|
|1| Criar sua conta|
|2| Criar Azure ML resource|
|3| Criar um laboratório|
|4| Criar e conectar a fonte de dados|
|5| Criar novo trabalho de ML automatizado|
|6| Implantar e testar o melhor modelo|
|7| Testar serviço implantado nos endpoints|

### Etapa 1 ao 5

Até a 3 etapa é simples, temos que apenas seguir as intruções e criar o ambiente virtual em que vamos trabalhar. Logo após isso vamos criar o autoML que juntamente se faz a criação e conecção com a fonte de dados. 

Para esse projeto, foi utilizado dados da [web](https://aka.ms/bike-rentals) para ser usado como dados de treinamento para o aprendizado da maquina. Como queremos um numero como resultado, foi utilizado tipo de **Aprendizagem de Máquina Supervisionada** do tipo **Regreção**, em que o rótulo (resultado) é um valor numérico.

Dutante a etapa 5 tamém é definido como serão os testes e quanto tempo duram. Nesse projeto por exemplo foi colocado que deveria durar até 15min todo o teste, caso não finalizado dentro do tempo, seria forçado a encerrar.

### Imprevistos :eyes: ⚠️

Por ser que ao gerar e testar seu autoML ele não encerre em 15min nem nunca. Nesse caso recomendo encerrar e refazer as 4 e 5 etapas .

### Etapa 6

Apos o autoML encerrar seu treinamento e aparecer o status concluido, irá abrir o melhor exemplo para usar as métricas dele como dados para criar um modelo de previsão. 

### Etapa 7

Após finalizado o modelo, vamos usalo para definir os pontos de extremidade (endpoints). Para isso, é selesionado as metricas e a implementação do modelo usando-as para criar os endpoints. Quando termina, a utima etapa é abrir os testes para testar os resultados e ver se estão corretos. 

### Dificuldades e Finalização 📍

Duante o processo obtive dificuldades em fazer os comandos funcionarem adequadamente. Pedi ajuda no foruum do bootcamp e obtive ajuda! Graças a eles e muito esforço consegui terminar o projeto. 



