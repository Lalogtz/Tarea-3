<img style="float: left; margin: 30px 15px 15px 15px;" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTFzQj91sOlkeDFkg5HDbjtR4QJYmLXkfMNig&usqp=CAU" width="400" height="500" /> 
    
    
### <font color='navy'> Simulación matemática. 

**Nombres:** Eduardo Gutiérrez Flores, Dario Castro Gonzales.

**Fecha:** 30 de octubre del 2022.

**Expediente** : 741305.
    
**Profesor:** Oscar David Jaramillo Zuluaga.
    
**Link Github**: Link con el enlace del repositorio del creador del proyecto

# Tarea 2: Clase 5
    
def g(x):
    return (5x^3 -3x + 10) 
df = sym.diff(f(x),x)
df
xc = sym.solve(df,x)
xc
f(0), f(10), f(1)

#Gráfica
xnum = np.linspace(0,10,254)
ynum = f(xnum)

# Crear el tamaño de la figura a graficar
plt.figure(figsize=(10,8))

#Agregar los gráficos
plt.plot(xnum,ynum,':y',lw=5,label='$y=x^2-2x+5$')
plt.plot([3],[8],'pr',ms=18,label='Punto máximo en el intervalo')
plt.plot([1],[4],'pg',ms=18,label='Punto mínimo en el intervalo')

#Nombrar los ejes de la gráfica
plt.xlabel('$x$',fontsize=18)
plt.ylabel('$y$',fontsize=18)

plt.grid()
plt.legend(loc='best')
plt.show()
