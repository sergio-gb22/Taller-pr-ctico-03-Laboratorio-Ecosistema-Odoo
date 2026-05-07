# Taller-practico-03-Laboratorio-Ecosistema-Odoo
## *Fase 1:* Integración de Módulos
Creo el archivo clientes_mock.csv y copio los datos dados en la actividad, para despues instalar la extension Rainbow CSV de visual studio code para que me muestre de una forma mas visible los datos resltandolos de colores, despues en el navegador busco LOCALHOST:8200 y entro como administrador para en la aplicación de ventas hacer Ventas > Pedidos > Clientes
e importar los registros darle a test y como me lo muestra todo en azul esta bien por lo que confirmo la importación dandole a importar, creo el producto con la cuenta de administrador

Despues entro con el usuario Comercial 01 y creo un presupuesto, en el pedido creo una factura 
<img width="802" height="900" alt="Captura" src="images/Captura de pantalla 2026-05-07 141427.png" />


## *Fase 2:* Elaboración de Informes
Tras activar el modo desarrollador voy a Ajustes > Técnico > Interfaz de Usuario > Vistas
en la barra de busqueda filtro por clave sale.report_saleorder_document, abro el xml y busco <div class="page"> para despues pegar el codigo:

<div class="row mt32 mb32" id="legal_warning">
    <div class="col-12">
        <p style="color: red; font-weight: bold; border-top: 1px solid black; padding-top: 10px;">
            Atención: Este documento vinculante está sujeto a las condiciones generales de venta de DAM/DAW S.L. (CIF: B-12345678).
        </p>
        <p class="text-muted" style="font-size: 10px; text-align: justify;">
            Protección de datos: En cumplimiento de la Ley Orgánica 3/2018 y el RGPD europeo, le informamos que sus datos serán tratados de forma estrictamente confidencial. Puede ejercer sus derechos ARCO dirigiéndose a nuestro DPO.
        </p>
    </div>
  </div>

  Tras guardar los cambios vuelvo a ventas y clico en el boton acción (que es la tuerca) y descargo el presupuesto del cliente en pdf
  pdf

  ## *Fase 3:* Exportación de Información
  Voy a la aplicación de facuración y Facturación > Clientes > Clientes marco la casilla del cliente clico en el boton acción (que es la tuerca) y selecciono exportar, selecciono que quiero "Exportar datos compatibles con importación" y de formato CSV despues en la columna izquierda, busca Nombre (name), Correo electrónico (email) y Teléfono (phone) y busca País (country_id), despliego y selecciono Nombre del país (country_id/name) y selecciono exportar donde se descargara el archivo

  
