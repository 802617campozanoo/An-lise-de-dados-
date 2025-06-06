# An-lise-de-dados-
Código para usar em análise de dados estatísticos 




import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns


dados = ['Azul', 'Vermelho', 'Azul', 'Verde', 'Vermelho', 'Azul']
frequencia = pd.Series(dados).value_counts()
print(frequencia)
