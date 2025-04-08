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




import matplotlib.pyplot as plt

label = ['a', 'b', 'c', 'd']
datos = [25, 35, 20 ,20]
colores = ['gold', 'lightcoral', 'lightskyblue', 'lightgreen']

plt.pie(datos, labels=label, colors=colores, autopct="%1.1f%%", startangle=140)
plt.axis("equal")
plt.show()
