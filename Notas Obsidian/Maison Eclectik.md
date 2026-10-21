## 1. Mapa de Procesos Operativos por Canal

### A. Canal de Venta Online (Ciclo de Vida de la Pieza)
1. *Captación / Adquisición:*
   * Fuentes de compra: Rastros, mercadillos, desembalajes, plataformas online (Vinted, Wallapop) y *House Markets / Ventas privadas en viviendas*.
   * Registro inicial del coste de compra, fecha y canal de procedencia.
2. *Acondicionamiento y Restauración:*
   * Limpieza profunda, puesta a punto y trabajos de restauración (cuando proceda).
3. *Investigación y Documentación:*
   * Búsqueda del origen de la pieza, época, atribución de autoría/estilo y hallazgos distintivos (ej. presencia de etiquetas originales).
   * Sesión de fotografía y catalogación visual.
4. *Tasación:*
   * Estimación del valor de mercado y fijación del precio estimado de venta.
5. *Logística de Almacén:*
   * Traslado físico de la pieza desde la vivienda/taller hasta el almacén.
6. *Publicación y Estado del Stock:*
   * Subida de la pieza a plataformas de venta (Vinted Pro, Wallapop, web, redes sociales).
   * El producto pasa a estado "A la espera / En venta".
7. *Procesamiento de Pedido y Envío:*
   * Confirmación de la venta -> Empaquetado y protección especial (piezas delicadas) -> Envío postal.
8. *Cobro y Liquidación:*
   * Transcurso del periodo de confirmación y cobro -> Recepción del dinero.

---

### B. Canal de Venta Presencial (Markets, Ferias y Eventos Pop-up)
1. *Gestión Organizativa:*
   * Inscripción, tramitación y pago de la reserva del puesto con la organización del evento.
2. *Comisariado de Selección:*
   * Selección en el almacén de los productos asignados para llevar al evento (según el perfil del público).
3. *Preparación y Materiales:*
   * Etiquetado individual de precios para el evento.
   * Acondicionamiento del atrezo del puesto: mesas, manteles, peanas, cartelería de marca y elementos decorativos.
4. *Logística y Transporte:*
   * Alquiler de furgoneta (si se precisa), carga de mercancía y traslado.
5. *Ejecución In Situ:*
   * Montaje del puesto, atención al público, venta y cobro presencial (efectivo, Bizum).
   * Desmontaje del puesto y recuento de mercancía al finalizar.
6. *Cierre Logístico:*
   * Devolución de la furgoneta alquilada y retorno del stock no vendido al almacén.

---

### C. Estrategia de Contenidos y Comunicación (Redes Sociales)
1. *Investigación:*
   * Búsqueda de curiosidades, contexto histórico de objetos y tendencias visuales para Reels/posts.
2. *Guionización:*
   * Estructuración de la narrativa, ganchos visuales y copies.
3. *Producción y Edición:*
   * Grabación de contenido (tours por mercadillos, hallazgos, procesos de transformación) y montaje/edición de vídeo.
4. *Atención a la Comunidad:*
   * Atención de dudas e interacciones directas vía mensaje privado (DMs) para ventas directas.

---

## 2. Sistema Contable, Tesorería y Gastos

### A. Ficha Financiera del Producto (Inventario)
Cada objeto registrado en la base de datos contará con los siguientes campos de seguimiento:
* *Fecha de Adquisición:* Día exacto de la compra.
* *Canal de Adquisición:* Rastro / Desembalaje / Vinted / Wallapop / House Market / Particular.
* *Coste de Adquisición:* Dinero pagado por la pieza.
* *Detalle de Etiqueta Original:* 
  * Indicador de si el objeto conserva la etiqueta original (Sí / No).
  * Notas sobre el precio original histórico o marca que figura en la etiqueta.
* *Gastos Directos Asociados:* Costes de restauración específica, piezas de recambio o portes aplicados directamente a esta pieza.
* *Valor Estimado de Venta (PVP Estimado):* Tasación inicial.
* *Valor Real de Venta (PVP Real):* Precio final tras el cierre o negociación.
* *Canal de Venta Final:* Market presencial, Vinted Pro, Wallapop, Instagram DM, Web.
* *Método/Vía de Cobro:* Efectivo, Bizum, Saldo Vinted, Transferencia bancaria.

---

### B. Control de Entradas y Salidas de Dinero (Cash Flow / Tesorería)
El sistema debe llevar el seguimiento del dinero en todas las bolsas/cuentas que maneja el negocio:
1. *Cuentas y Fuentes Registradas:*
   * *Caja / Efectivo:* Entradas por ventas presenciales en markets; salidas por compras de stock en metálico (rastros, House Markets).
   * *Bizum / Cuenta Bancaria:* Entradas por ventas directas o transferencias bancarias.
   * *Saldos en Plataformas (Vinted / Wallapop):* Entradas por ventas cobradas en la plataforma; salidas cuando se compra stock nuevo usando ese mismo saldo.

2. *Gestión de Gastos Operativos e Indirectos:*
   * *Gastos de Limpieza, Restauración y Taller:*
     * Distinción del gasto: *Con Factura* (deducible fiscalmente) vs. *Sin Factura / Ticket* (descuenta solo del margen real interno).
     * Imputación: Asignación como Gasto Directo (a una pieza concreta) o como Gasto Fungible/General (productos de taller compartidos como alcohol, ceras, disolventes o trapos).
   * *Gastos de Markets:* Alquileres de puesto, alquiler de furgoneta, gasolina, dietas, peajes y atrezo/decoración del estand (manteles, mesas, cartelería).
   * *Suministros de Embalaje:* Cajas compradas al por mayor, cinta de embalar, plástico de burbujas, etiquetas.

---

## 3. Funcionalidades Requeridas para el Desarrollo de la App

* *Gestión de Estados del Producto:* Flujo visual para mover la pieza a lo largo de su ciclo:
  Comprado ➔ En Restauración ➔ En Almacén ➔ Asignado a Market / En Venta Online ➔ Vendido
* *Calculadora Automática de Margen Neto:* Cálculo automático por cada objeto:
  $$\text{Margen Neto} = \text{Precio Real Venta} - (\text{Coste Adquisición} + \text{Gastos Directos} + \text{Comisiones/Gastos Envío})$$
* *Control de Stock Multicanal:* Consultar al instante qué piezas están en el almacén, cuáles están reservadas para un market presencial y cuáles están publicadas online para evitar ventas dobles.
* *Cuadro de Mando Financiero (Dashboard):*
  * Resumen de entradas y salidas diferenciadas por método de pago (Efectivo vs. Digitales).
  * Impacto del margen *Fiscal* (solo facturas) vs. *Margen Real* (facturas + tickets/gastos sin factura).
  * Valor del stock total acumulado en el almacén esperando venta.
  * Balance de beneficio neto mensual.