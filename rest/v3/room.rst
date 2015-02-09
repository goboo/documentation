GET /api/v3/rest/room/{room}.json
=================================

Fetch details of a specific room.

+------------+-----------------------------------+
| Method     | ``GET``                           |
+------------+-----------------------------------+
| URL        | ``/api/v3/rest/room/{room}.json`` |
+------------+-----------------------------------+
| ``{room}`` | ID or slug of the room.           |
+------------+-----------------------------------+

Response example
----------------

.. code:: json

   {
       "id": "491fb5a9-974e-11e4-b6e8-001c426331bc",
       "slug": "demo",
       "title": "Demo",
       "capacity": 16,
       "timeOffset": 6,
       "modes": []
   }
