# lazyLoading
Ejercicio de Lazy loading
Hola, mi nombre es Jhonatan Villanova. Soy un ingeniero de Sistemas de nacionalidad Colombiana, estoy haciendo una serie de 
ejercicios para nutrir mis habilidades como desarrollador.
Hago uso de lazy loading, una interesante forma de optimizar la carga de imagenes, videos e iframes con los que disminuimos la 
carga inicial consumiendo sólo las peticiones para cargar la página y el contenido minimamente necesarios y el resto es cargado
conforme el usuario lo necesita.

En este ejercicio, hice uso del atributo loading que al parecer debería tener soporte en todos los navegadores pero no funciona 
igual en Chrome. 
Chrome al parecer buscar cargar toda la información lo más rápido posible por lo que el loading lazy no tiene
el mismo resultado. En Firefox el lazy loading funciona perfectamente.
Una de las formas de optimizacion es comprimir el peso de las imagenes por medio de una aplicacion o compresor, para este caso
utilice TinyPNG como compresor con el fin de reducir el tiempo de carga, otra de las formas de optimizar estos tiempos es
utilizar el tamaño de la imagen que necesitamos, si queremos una imagen de 80px pero cargamos una de 2000px estamos haciendo un
uso ineficiente de nuestros recursos.


Para ponernos en datos, la carga inicial de las imágenes era de 44 MB pero al utilizar un compresor el tamaño de las peticiones
pasó a 9.4 MB. Esto en Chrome donde lazy load no funciona correctamente, en navegadores como Firefox el lazy nos permite disminuir
incluso más la carga inicial. En números reducimos la carga un 78.6% sólo utilizando un programa de compresión. 
