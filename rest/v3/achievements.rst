GET /api/v3/rest/room/{room}/achievements.json
==============================================

Fetch achievements configured in a room and players that have received them.

+------------+------------------------------------------------+
| Method     | ``GET``                                        |
+------------+------------------------------------------------+
| URL        | ``/api/v3/rest/room/{room}/achievements.json`` |
+------------+------------------------------------------------+
| ``{room}`` | ID or slug of the room.                        |
+------------+------------------------------------------------+

Response example
----------------

.. code:: json

   [
       {
           "players": [
               "Master Player",
               ...
           ],
           "id": "492c62cf-8d78-11e3-ba00-12b9e596cdaa",
           "title": "3 Spiele nacheinander",
           "slug": "3er-serie"
       },
       ...
   ]
