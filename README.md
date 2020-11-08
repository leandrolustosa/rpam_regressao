Em um jupyter notebook:

1. Carregue uma base de dados de regressão que NÃO esteja nos toy datasets do scikit-learn;
- Dataset escolhido (Kaggle): BMW - 100,000 UK Used Car Data set
- Link: https://www.kaggle.com/adityadesai13/used-car-dataset-ford-and-mercedes
- O modelo "4 Series" da BMW foi o escolhido, porque eu gostei mais desse modelo e ele tinha próximo de 1000 registros (995)
- A coluna "price" é o target.
- As colunas transmission e fuelType eram texto, foram transformadas em número.
- Removi a coluna "model" do dataset, pois estou trabalhando com apenas um modelo
- Após todo o pré processamento da base de dados o dataset ficou da seguinte forma:

    995 registros e um total de 8 colunas:

    | #   | Column       | Non-Null Count | Dtype   |
    | --- | ------------ | -------------- | ------- |
    |  0  | year         | 995 non-null   | int64   |
    |  1  | transmission | 995 non-null   | int32   |
    |  2  | price        | 995 non-null   | int64   |
    |  3  | mileage      | 995 non-null   | int64   |
    |  4  | fuelType     | 995 non-null   | int32   |
    |  5  | tax          | 995 non-null   | int64   |
    |  6  | mpg          | 995 non-null   | float64 |
    |  7  | engineSize   | 995 non-null   | float64 |

2. Treine um modelo da classe LinearRegression do scikit-learn com toda a base;
3. Calcule o MSE (erro quadrático médio) para todos os exemplos da usada como treino no modelo treinado;
4. Plote em um gráfico (2D) o MSE em função do atributo intercept_ da classe LinearRegression. Mantenha os valores do atributo coef_ fixos e varie o valor de intercept_ entre intercept_ - delta e intercept_ + delta. O gráfico tem que ser uma parábola com concavidade para cima. Não plote um gráfico 3D com visão de cima.
