.. Copyright (c) 2007-2016 UShareSoft, All rights reserved

.. _userTargetPlatforms-getAll:

userTargetPlatforms_getAll
--------------------------

.. function:: GET /users/{uid}/targetplatforms

.. sidebar:: Summary

	* Method: ``GET``
	* Response Code: ``200 / 304``
	* Response Formats: ``application/xml`` ``application/json``
	* Since: ``UForge 3.6``

Retrieves all the target platforms available for an user. 

A list of :ref:`targetplatform-object` objects are returned. 

You can use a ``search criteria`` to retrieve a subset of these target platforms. 

.. warning:: The target platforms available for a user not only depends on the access rights given for the user but also the access rights of the target platform in the organization.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``appliance_create``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the id of the :ref:`user-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "http://www.example.com/api/users/{uid}/targetplatforms" -X GET \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`targetformat-api-resources`
	 * :ref:`targetplatform-api-resources`
	 * :ref:`imageformat-object`
	 * :ref:`targetformat-object`
	 * :ref:`targetplatform-object`
	 * :ref:`userFormats-getAll`
	 * :ref:`userFormats-update`
	 * :ref:`userTargetFormat-getAll`
	 * :ref:`userTargetFormat-update`
	 * :ref:`userTargetPlatforms-update`
	 * :ref:`userTargetPlatformFormat-getAll`