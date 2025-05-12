Numpy:
import numpy as np
datos = np.array([10, 20, 30, 40, 50])
media = np.mean(datos)
std = np.std(datos, ddof=1)
varianza = np.var(datos, ddof=1)
mediana = np.median(datos)
print(datos)
print(media)
print(std)
print(varianza)
print(mediana)


Scipy:
from scipy 
import stats
datos = [10, 20, 30, 40, 50]
media = stats.tmean(datos)
std = stats.tstd(datos)
varianza = stats.tvar(datos)
mediana = stats.scoreatpercentile(datos, 50)
print(datos)
print(media)
print(std)
print(varianza)
print(media)
