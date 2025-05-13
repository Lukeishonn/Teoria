import pandas as pd
df = pd.read_csv("users.csv")
mayores_50 = df[df['edad'] > 50]
masculinos = mayores_50[mayores_50['genero'].str.lower() == 'male']['nombre']
femeninos = mayores_50[mayores_50['genero'].str.lower() == 'female']['nombre']
print("Nombres de usuarios masculinos de 50: ")
print(masculinos)
print("Nombres de usuarios femeninos de 50: ")
print(femeninos)




import pandas as pd
import matplotlib.pyplot as plt



df = pd.read_csv("users.csv")

mayores_50 = df[df['edad'] > 50]
conteo_genero = mayores_50['genero'].str.lower().value_counts()

plt.figure(figsize=(6, 4))
conteo_genero.plot(kind='bar', color=['pink', 'blue'])
plt.title("Usuarios mayores de 50 años Masculinos y Femeninos")
plt.xlabel("Genero")
plt.ylabel("Cantidad de usuarios")
plt.xticks(rotation=0)
plt.tight_layout()
plt.show()
