## Proyecto Brazilian Ecommerce

### Problema de negocio
Aumento de insatisfacción de clientes en reseñas de baja calificación en una plataforma de comercio electrónico

### Propuesta de solución
Realizar un levantamiento de los pedidos con respecto a los puntos de entrega y planificar los despachos considerando la cantidad, destino, capacidad y monto de los pedidos de los clientes. De esta manera, se podrá mejorar la atención on time/in full a los clientes.

### Descripción datasets

#### Dataset: Customers

El conjunto de datos "customers" contiene información detallada sobre los clientes de un comercio electrónico. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **customer_id:** Identificador único asignado a cada cliente.
- **customer_unique_id:** Identificador único y persistente asociado a cada cliente.
- **customer_zip_code_prefix:** Prefijo del código postal del cliente.
- **customer_city:** Ciudad donde reside el cliente.
- **customer_state:** Estado en el que se encuentra ubicado el cliente.

#### Dataset: Geolocation

El conjunto de datos "geolocation" proporciona información geográfica detallada asociada a códigos postales. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **geolocation_zip_code_prefix:** Prefijo del código postal asociado a la ubicación geográfica.
- **geolocation_lat:** Latitud de la ubicación geográfica.
- **geolocation_lng:** Longitud de la ubicación geográfica.
- **geolocation_city:** Ciudad correspondiente a la ubicación geográfica.
- **geolocation_state:** Estado en el que se encuentra ubicada la geolocalización.

#### Dataset: Order Items

El conjunto de datos "order_items" contiene información detallada sobre los productos incluidos en cada pedido. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **order_id:** Identificador único del pedido.
- **order_item_id:** Identificador único del ítem dentro del pedido.
- **product_id:** Identificador único del producto.
- **seller_id:** Identificador único del vendedor asociado al producto.
- **shipping_limit_date:** Fecha límite de envío del pedido.
- **price:** Precio del producto.
- **freight_value:** Valor del flete asociado al envío.

#### Dataset: Order Payments

El conjunto de datos "order_payments" proporciona información detallada sobre los pagos asociados a cada pedido. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **order_id:** Identificador único del pedido.
- **payment_sequential:** Número de secuencia del pago dentro del pedido.
- **payment_type:** Tipo de pago utilizado para la transacción.
- **payment_installments:** Número de cuotas en las que se dividió el pago.
- **payment_value:** Valor total del pago asociado al pedido.

#### Dataset: Order Reviews

El conjunto de datos "order_reviews" contiene información detallada sobre las revisiones y comentarios realizados por los clientes sobre sus pedidos. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **review_id:** Identificador único de la revisión.
- **order_id:** Identificador único del pedido asociado a la revisión.
- **review_score:** Puntuación otorgada por el cliente al pedido (escala del 1 al 5).
- **review_comment_title:** Título del comentario dejado por el cliente.
- **review_comment_message:** Mensaje detallado del comentario realizado por el cliente.
- **review_creation_date:** Fecha en que se creó la revisión.
- **review_answer_timestamp:** Marca de tiempo de la respuesta a la revisión.

#### Dataset: Orders

El conjunto de datos "orders" proporciona información detallada sobre los pedidos realizados por los clientes. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **order_id:** Identificador único del pedido.
- **customer_id:** Identificador único del cliente que realizó el pedido.
- **order_status:** Estado actual del pedido (por ejemplo, "delivered" para entregado).
- **order_purchase_timestamp:** Marca de tiempo de la compra del pedido.
- **order_approved_at:** Marca de tiempo en que el pedido fue aprobado.
- **order_delivered_carrier_date:** Fecha en que el pedido fue entregado al transportista.
- **order_delivered_customer_date:** Fecha de entrega del pedido al cliente.
- **order_estimated_delivery_date:** Fecha estimada de entrega del pedido.

#### Dataset: Product Category Translation

El conjunto de datos "prod_cat_translation" proporciona la traducción de las categorías de productos a inglés. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **product_category_name:** Nombre de la categoría de productos en el idioma original.
- **product_category_name_english:** Nombre de la categoría de productos traducido al inglés.

#### Dataset: Products

El conjunto de datos "products" contiene información detallada sobre los productos disponibles. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **product_id:** Identificador único del producto.
- **product_category_name:** Categoría a la que pertenece el producto.
- **product_name_length:** Longitud del nombre del producto.
- **product_description_length:** Longitud de la descripción del producto.
- **product_photos_qty:** Cantidad de fotos asociadas al producto.
- **product_weight_g:** Peso del producto en gramos.
- **product_length_cm:** Longitud del producto en centímetros.
- **product_height_cm:** Altura del producto en centímetros.
- **product_width_cm:** Ancho del producto en centímetros.

#### Dataset: Sellers

El conjunto de datos "sellers" proporciona información sobre los vendedores asociados a los productos. A continuación, se presenta una descripción de las columnas presentes en este dataset:

- **seller_id:** Identificador único del vendedor.
- **seller_zip_code_prefix:** Prefijo del código postal del vendedor.
- **seller_city:** Ciudad donde se encuentra ubicado el vendedor.
- **seller_state:** Estado en el que se encuentra ubicado el vendedor.
