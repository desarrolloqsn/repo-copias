# PROCEDIMIENTO PARA DEJAR EL REPOSITORIO LISTO

# 1 - MODIFICAMOS EL NOMBRE DEL DASHBOARD:  Una vez Clonado el repositorio y abierto el proyecto en nuestro ide debemos ir a la carpeta contenedores/Dashboard/Filtro 
## alli cambiaremos el nombre del dashboard en la linea 533  y guardamos los cambios 

# 2 - MODIFICAMOS EL USUARIO Y CONTRASEÑA : para modificar el usuario y contraseña nos debemos dirigir a -> /componentes/Formularios/index.jsx en la linea 29
## modificamos el usuario y la contraseña y guardamos los cambios con ctrl + s

# 3 :  MODIFICAMOS LA DIRECCION DE LOS GRAFOS: 
# a -> src/componentes/Graficos/GrafoComunidadesEnRedes.jsx en la linea 281 https://qsngrafos.vercel.app/comunidades/+id_cliente 
# b -> src/componentes/Graficos/GrafoComunidades.jsx en la linea 51 https://qsngrafos.vercel.app/comunidades/+id_cliente
# c -> src/componentes/Graficos/GrafoComunidadesEnRedes.jsx en la linea 233 https://qsngrafos.vercel.app/comunidades/+id_cliente
# d -> src/componentes/Graficos/grafoPalabrasMasFrecuentes.jsx en las lineas 209,219,228,246,256 y 266 modificar https://qsngrafos.vercel.app/palabras/+id_cliente
# e -> src/componentes/Graficos/GrafosModelos.jsx en las lineas 64,74,84,95,105,115 https://qsngrafos.vercel.app/palabras/+id_cliente

# comandos basicos para commitear y pushear en git
# ctrl + shift + ñ (para abrir terminal)
# a- git pull (para asegurarnos de traernos los cambios  que otros pueden haber subido)
# b- git add . (para agregar todos los archivos que hemos modificado)
# c - git commit -m "Mensaje explicando lo que hemos hecho"
# d - git push origin master (para enviar los cambios a github)

# PARA DEPLOYAR EN VERCEL
#  -> https://vercel.com : verificamos que estamos en la cuenta pro de qsocial damos a -> add new -> project -> import git -> importamos nuestro proyecto -> proyect name -> framewok (Create React App) -> build and Output Settings (damos al boton de "OVERRIDE" y dentro del input escribimos " CI= npm run build" y guardamos)-> Enviroment Variables (creamos estas tres variables NODE_OPTIONS  --max-old-space-size=4096, GENERATE_SOURCEMAP  false, CI= false) -> deployd