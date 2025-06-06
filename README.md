# An-lise-de-dados-
Código para usar em análise de dados estatísticos 


import pandas as pd

dados = ['Azul', 'Vermelho', 'Azul', 'Verde', 'Vermelho', 'Azul']
frequencia = pd.Series(dados).value_counts()
print(frequencia)


import numpy as np

idades = np.array([18, 21, 22, 19, 20, 22])
print("Média das idades:", idades.mean())



notas = np.array([[7.5, 8.0, 9.0], [6.0, 7.5, 8.5]])
print("Formato da matriz (linhas, colunas):", notas.shape)


dados = pd.DataFrame({
    'Nome': ['Ana', 'Carlos', 'Beatriz'],
    'Idade': [22, 23, 21],
    'Renda': [2500, 3000, 2800]
})
print(dados.describe())


import seaborn as sns
import matplotlib.pyplot as plt

df = pd.DataFrame({
    'Setor': ['TI', 'TI', 'RH', 'RH', 'Vendas', 'Vendas'],
    'Salario': [5000, 5200, 3000, 3100, 4000, 4200]
})
sns.boxplot(x='Setor', y='Salario', data=df)
plt.title("Distribuição de Salários por Setor")
plt.show()


escolas = {
    "Escola A": [8.0, 7.5, 9.0],
    "Escola B": [6.5, 7.0, 6.0]
}
print("Notas da Escola A:", escolas["Escola A"])




estatisticas = {
    "media": np.mean(idades),
    "desvio_padrao": np.std(idades),
    "mediana": np.median(idades)
}
print(estatisticas)

