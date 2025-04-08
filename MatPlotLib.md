import matplotlib.pyplot as plt

#datos
x = [1, 2, 3, 4, 5]
y = [10, 20, 30, 40, 50]

#Crear grafico
plt.plot(x, y)

#etiqueta de texto
plt.xlabel("Eje x: ")
plt.ylabel("Eje y: ")
plt.title("Grafico de ejemplo: ")

#mostrar
plt.show()
