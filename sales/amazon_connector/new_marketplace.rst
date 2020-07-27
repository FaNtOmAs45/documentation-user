======================================================
Add an unsupported marketplace to the Amazon Connector
======================================================

Some newer Amazon Marketplaces, such as Amazon Brazil or Amazon Netherlands, are
not included by default in the Amazon Connector list of possible marketplaces.

These marketplaces can be added manually should you wish to use them.

.. warning::
    These marketplaces are not officially supported by Odoo - there is no guarantee
    that adding a new marketplace as described here will work, nor can this be considered
    as a bug when contacting Odoo Support.

.. note::
    Amazon marketplaces are only supported in the European and North American region;
    though Amazon includes Brazil with the North American region and India in the
    European region, so your mileage may vary.

To add a new marketplace, you must first enable 
:doc:`Developer mode <../../general/developer_mode/activate>`.

Once that is done, go to :menuselection:`Sales --> Configuration --> Settings --> Connectors --> Amazon Sync -->
Amazon Marketplaces`.

From there, you can create a new marketplace record. You will need the Marketplace ID and Endpoint for your
marketplace as described in the
`Amazon Documentation <https://docs.developer.amazonservices.com/en_US/dev_guide/DG_Endpoints.html>`_.

Set the name of the record to ``Amazon.<domain>`` to easily retrieve it. The **Code**, **Domain** and
**API Identifier** fields should contain the *Country Code*, *Amazon MWS Endpoint* and *MarkteplaceId*
values from the Amazon Documentation respectively.

Once the marketplace is saved, you should then update the Amazon Account configuration by going to 
:menuselection:`Sales --> Configuration --> Settings --> Connectors --> Amazon Sync --> Amazon Accounts`,
open the account on which you wish to use the new marketplace, go to the **Marketplaces** tab and click
on **Update available marketplaces** (an animation should confirm the success of the operation). You can then
edit the Amazon Account to add the new marketplace in the list of synchronized marketplaces - if the new
marketplace is not available in the list, it means it is either incompatible with the account's region or
simply that it is not supported by the Amazon Connector.