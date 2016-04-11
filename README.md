# 11.abril.2016
repaso de clases

## repaso ##

# generar una base de datos y declarar data.frame 
# que es un data.frame en R??
# para que es la c abtes de meter los daros, c()??
# es importante cambiar una variable a numerico? porque?

nombres <- c("rodolfo", "angel", "alejandro")
prepa <- c("UNO", "DOS", "TRES")

## IMPORTAMOS BASE DE DATOS
require (foreign)
baseinegi <- read.dbf("ubicacion con coble diagonal y al final doblediagonal el nombre del archivo . dbf")

##cambiar a numerico la variable
baseinegi$algonuevo <- as.numeric(as.character(baseinegi$algo))
baseinegi$otroalgonuevo <- as.numeric(as.character(baseinegi$otroalgo))

## uso del subset (para elegir solo algunos casos)

precod <- subset(nombrebase, ((variable1 == a) & (variable2 == b) & (variable3 ==a | varioable3 == b)), 
                 select = c(variable1, variable2, varibalw3)
                 ### select es para seleccionar las colunas que quiere que muestre
                   
attach(nombre base) # a partis de esta linea ya solo trabajas con la base que quieres y asi ya solo puedes llamar la variable
nombrebase seguidode la variable <- table (nombre base)
detach # a partir de aqui ya no voy a trabajar con esa base

## graficas
# con nombre de la grafica, nombre en los limites, limites de los ejes, color, pch, border, etc
# el color puede ser asi c(2, 13, 16) o con el nombre entre comillas

# questionr
install.packages("questionr")
require (questionr)
c <- wtd.table(sdemt$varible, weights=sdemt$otravariable) ## factor de expansion
## paqueteria para ponderar casos

##ponderar casos y sacar porcentajes
tabarama <- wtd.table(sdemt$varible,sdemt$varible1, weights=sdemt$otravariable)
c1.1 <- round(tabarama/margin.table(tabarama)*100,2) ## ,2 decimales

## exportar con .csv, si lo hacemos en un solo libro diferentes hojas puntos extras

##etiquetar
sdemt$variable <- ordered (sdemt$variable, levels = c(1,2), labels = c("h", "m"))


##recodificar
# metodo 1 y metodo 2

## series de tiempo ##

# simular una serie de tiempo
desoc <- sample(3:8,44, raplece = T)
TDESOC <- ts(desoc, frequency = 12, start= 2010)

## graficar serie de tiempo
plot(ST, xlab... , ylab..., main =...)

##serie de tiempo multiple ##
prof <- sample(5:8, 60, replace = T)
y asi todas mis series o tambien
prof1 <- ts(base[renglon,columna], frequency = , start = )
seriemultople <- ts.intersect(prof1, serie2, serie3 y asi)
## ¡describe tres argumentos de la funcion ts.intersec
help(ts.intersect)

##separar serie de tiempo

nuevo_nombre <- window(base, start = c(año, periodo), end=c (año,periodo))
plot(nombre_serie, main = "nombre", xlab = "nombre", ylab = "nombre")
                       
                           
## para saber donde empieza y donde termina
start(base)
end (base)

##descomposicion de st
ts.des <- decompose(base en ts) ## por default es el modelo aditivo
names()

## para la autocorrelacion
require (forecast)
require (fpp)
Acf
      
