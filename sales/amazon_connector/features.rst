=======================================
Synchronization between Amazon and Odoo
=======================================

The **Amazon Connector** synchronizes the orders between Amazon and your Odoo database, which
reduces considerably the amount of time spent on your Amazon Marketplace dashboard, making your
daily routine a lot easier. More advanced tasks still require you to connect to your Amazon account.

This connector is able to:

+--------------------------------------------------+----------------------------------------+
| From Amazon to Odoo                              | From Odoo to Amazon                    |
+==================================================+========================================+
| Synchronize all confirmed orders (both FBA and   | Notify Amazon of a confirmed shipping  |
| FBM) and their order items which include:        | (FBM) in order to get paid.            |
|                                                  |                                        |
| - the product's details (SKU, listing name &     |                                        |
|   description, quantity, etc.)                   |                                        |
| - the shipping costs for the product             |                                        |
| - the gift wrapping charges                      |                                        |
+--------------------------------------------------+----------------------------------------+
| Create any missing offer related to an order.    | Notify Amazon of a manually canceled   |
|                                                  | order (This feature has been dropped   |
|                                                  | in Odoo 13.1 and higher versions)      |
+--------------------------------------------------+----------------------------------------+
| Create any missing partner related to an order   |                                        |
| (contact types supported: contact and delivery). |                                        |
+--------------------------------------------------+----------------------------------------+

.. note::
   The connector handles the features listed above only and nothing else.

.. seealso::
   - :doc:`apply`
   - :doc:`setup`
   - :doc:`manage`

