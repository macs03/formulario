formulario
==========

formulario para Inventr

1 Parte : Debe ser un formulario usando los elementos del bootstrap input text y botones y en la zona de eventos debe imprimir los eventos registrados en el formulario 2 para que se puedan seleccionar con checks. 

	Acciones. Al darle click sobre el boton de guardar por medio de jquery debe hacer un envio Get de la información a otra pagina en php con los valores que estan dentro del formulario. en la pagina de php debe realizar la acción que necesite bien sea Guardar , Modificar , Eliminar. el php le debe responder preferiblemente un objeto Json con un estatus de la acción ejemplo

Status
1 . Si guardo con exito
2. Si en caso de guardar el código ya se encuentra registrado. 

	Luego de recibir la respuesta con jquery debe mostrar el mensaje si se ejecutó con éxito la acción o existe algún error, y verificar las acciones que necesita realizar por ejemplo si la acción fue eliminar el formulario debe quedar vacio solo esperando datos para realizar un registro nuevo. 



2 Parte:   Esta sera la parte de la busqueda de cada uno de los registros, debe paginar de 3 registros por pagina, la parte de busqueda debe funcionar con un like de sql buscando en cada uno de los 3 campos por si hay alguna coincidencia, no se necesita tener la informacion completa por ejemplo : Evento Numero uno San juan de Colon   al realizar la busqueda solo podria escribir San juan de Colon y el sistema  deberia mostrarme ese resultado. preferiblemente que la pagina no sea recargada en su totalidad para hacer esto solo que se interactúe en esta zona con jquery sin que toda la página sea recargada. 


El principio funcional del sistema sería un evento en el cual podrán existir zonas  Vip, Platinium  entre otras estas, las zonas pueden variar por evento por lo que en el registro de los eventos se debe permitir la seleccion de varias zonas por evento.

En cada una de las zonas existen diferentes tipo de mesas ejemplo en las zonas Vip puede tener Mesas de 4 Personas y de 8 personas pero en la zona platinium solo mesas de 8 por lo que en el registro de las zonas se puede seleccionar las mesas que tiene esa zona

Las mesas como se vera a continuacion solo tendran un codigo y la cantidad de personas máximas que pueden tener. 


Todos los registros se deben manejar bajo la misma forma de trabajo tiene libertad de diseño usando el bootpstrap pero sin pasar por alto el principio funcional que se le esta pidiendo .

Descripción de la data. 

1 Evento Codigo  (Unico) (Requerido)
2 Descripción del Evento (Requerido)
3 Lugar del Evento 
4 Fecha del Evento (Requerido)(Validar Fecha)
5 Fecha Inicio  Venta (Requerido)(Validar Fecha)
6 Zona de Eventos 

No pueden existir eventos con el mismo Código


Para las zonas

1 Zona Codigo  (Unico) (Requerido)
2 Descripción de la Zona (Requerido)
3 Mesas Permitidas en la Zona


Para las Mesas

1 Mesa Codigo  (Unico) (Requerido)
2 Descripción de la Mesa (Requerido)
3 Cantidad de personas  Permitidas (Requerido)(Validar Numero)
