GET /api/v3/rest/rooms.json
===========================

List all rooms that are defined and published in the GoBoo&reg; system.

+--------+-----------------------------+
| Method | ``GET``                     |
+--------+-----------------------------+
| URL    | ``/api/v3/rest/rooms.json`` |
+--------+-----------------------------+

Response example
----------------

.. code:: json

   [
       {
           "id": "491fb5a9-974e-11e4-b6e8-001c426331bc",
           "slug": "demo",
           "title": "Demo",
           "capacity": 16,
           "timeOffset": 6,
           "modes": []
       }
   ]
