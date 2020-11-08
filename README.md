Em um jupyter notebook:

1. Carregue uma base de dados de regressão que NÃO esteja nos toy datasets do scikit-learn;
2. Treine um modelo da classe LinearRegression do scikit-learn com toda a base;
3. Calcule o MSE (erro quadrático médio) para todos os exemplos da usada como treino no modelo treinado;
4. Plote em um gráfico (2D) o MSE em função do atributo intercept_ da classe LinearRegression. Mantenha os valores do atributo coef_ fixos e varie o valor de intercept_ entre intercept_ - delta e intercept_ + delta. O gráfico tem que ser uma parábola com concavidade para cima. Não plote um gráfico 3D com visão de cima.
