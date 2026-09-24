# 📊 Modelo de Previsão com Microsoft Azure

Este repositório contém o projeto prático de criação de um modelo de previsão utilizando os recursos de **Machine Learning** da Microsoft Azure, desenvolvido como parte de um desafio da [DIO](https://www.dio.me/).

O objetivo principal é explorar os conceitos de Inteligência Artificial e Machine Learning Automatizado (AutoML), criando um modelo do zero e disponibilizando seus pontos de extremidade (endpoints) para consumo.

---

## 🚀 Passo a Passo do Desenvolvimento

*Abaixo está o racional utilizado para a criação e implantação do modelo:*

1. **Criação do Workspace:** 
   Iniciei criando um recurso de *Azure Machine Learning* no portal do Azure, configurando o grupo de recursos e o workspace.
2. **Configuração de Computação:** 
   Instanciei um cluster de computação adequado para rodar o treinamento do modelo sem gargalos.
3. **Criação do Ativo de Dados (Dataset):** 
   Fiz o upload da base de dados fornecida e a registrei como um ativo de dados no Machine Learning Studio.
4. **Treinamento com Automated ML:** 
   Configurei um novo trabalho de ML Automatizado, selecionando a coluna alvo (target) e o tipo de tarefa (ex: Regressão ou Classificação). Deixei o Azure testar os melhores algoritmos.
5. **Avaliação das Métricas:** 
   Após o término do treinamento, acessei a aba de modelos e analisei as métricas (como *Normalized Root Mean Squared Error*) do melhor algoritmo escolhido pela plataforma.
6. **Implantação (Deploy) e Teste:** 
   Realizei o deploy do modelo vencedor, gerando um endpoint REST em tempo real. Por fim, testei o endpoint enviando um payload JSON e verificando a resposta da previsão.

---

## 📂 Arquivos do Projeto

- `README.md`: Documentação com o passo a passo do processo (este arquivo).
- `endpoints.json`: Arquivo contendo as configurações, chaves e a URL do ponto de extremidade gerado pelo Azure. *(Certifique-se de fazer o upload desse arquivo neste repositório)*.

---

## 🔗 Links e Referências Importantes

Durante o desenvolvimento deste projeto, as seguintes documentações foram utilizadas como base:

- [Explore Azure AI Services](https://learn.microsoft.com/pt-br/azure/ai-services/)
- [Explore Automated Machine Learning in Azure Machine Learning](https://learn.microsoft.com/pt-br/azure/machine-learning/concept-automated-ml)

---

Desenvolvido com dedicação para a expansão do portfólio de projetos técnicos! 😎🚀
