#### ¿Cuándo usar el gancho useSearchParams() frente a la propiedad searchParams?

Es posible que haya notado que usó dos formas diferentes de extraer parámetros de búsqueda.
El uso de uno u otro depende de si se trabaja en el cliente o en el servidor.

- **\<Search>** es un componente de cliente, por lo que utilizó el enlace para acceder a los parámetros desde el cliente.useSearchParams()

- **\<Table>** es un componente de servidor que obtiene sus propios datos, por lo que puede pasar la propiedad de la página al componente.searchParams

Como regla general, si desea leer los parámetros del cliente, use el gancho **"useSearchParams()"** ya que esto evita tener que volver al servidor.
