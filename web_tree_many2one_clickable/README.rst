Clickable many2one fields for tree views
========================================

This addon provides a separate widget to allow many2one fields in a tree view
open the linked resource when clicking on their name.

You can also define a system parameter to have this behaviour for all the
existing many2one fields in tree views.

Installation
============

Install it the regular way.

Configuration
=============

If you want to have all many2one fields clickable by default, you have to
define in *Configuration > Technical > Parameters > System parameters*, a new
parameter with name `web_tree_many2one_clickable.default` and with value
`true`.

Usage
=====

For the widget option, you need to add `widget="many2one_clickable"` attribute
in the XML field definition in the tree view.

For example:

`<field name="partner_id" widget="many2one_clickable" />`

will open the linked partner in a form view.

Known issues / Roadmap
======================

* You cannot deactivate clickable behaviour for an specific many2one field if
  you configure the system parameter.
* The value of the system parameter is retrieved for each many2one field
  present in the view instead of only once.

Credits
=======

Contributors
------------

* Therp BV
* Pedro M. Baeza <pedro.baeza@serviciosbaeza.com>

Maintainer
----------

.. image:: http://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: http://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

To contribute to this module, please visit http://odoo-community.org.
