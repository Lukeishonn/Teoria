import matplotlib.pyplot as plt 
import pandas as pd 
df = pd.read_csv("users.csv") 
df_espana = df[df['pais'] == 'Spain']
print(df_espana)
genero_counts = df_espana['genero'].value_counts()
print(genero_counts)
genero_counts.plot(kind='bar', color=['pink', 'blue'])
plt.title('Cantidad de Hombres y Mujeres en España') 
plt.ylabel('Genero')
plt.xlabel('cantidad')
plt.show()
