.. Copyright (c) 2007-2016 UShareSoft, All rights reserved

.. _projectLicense-download:

projectLicense_download
-----------------------

.. function:: GET /distributions/{id}/projects/{pid}/licenses/{lid}

.. sidebar:: Summary

	* Method: ``GET``
	* Response Code: ``200 / 304``
	* Response Formats: ``*/*``
	* Since: ``UForge 1.0``

Downloads the license of a project.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``appliance_create``

URI Parameters
~~~~~~~~~~~~~~

* ``lid`` (required): the id of the :ref:`license-object`
* ``pid`` (required): the id of the :ref:`project-object`
* ``id`` (required): the id of the :ref:`distribprofile-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "http://www.example.com/api/distributions/{id}/projects/{pid}/licenses/{lid}" -X GET \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`project-object`
	 * :ref:`license-object`
	 * :ref:`projectLicense-download`
	 * :ref:`projectLicense-upload`
	 * :ref:`projectLicense-uploadChunk`
	 * :ref:`projectLicense-delete`