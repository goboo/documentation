GET /api/v3/rest/room/{room}/slot/{slot}.json
=============================================

Fetch details of a specific slot.

+------------+---------------------------------------------------------------------+
| Method     | ``GET``                                                             |
+------------+---------------------------------------------------------------------+
| URL        | ``/api/v3/rest/room/{room}/slot/{slot}.json``                       |
+------------+---------------------------------------------------------------------+
| ``{room}`` | ID or slug of the room.                                             |
+------------+---------------------------------------------------------------------+
| ``{slot}`` | ID of the slot, or one of ``current``, ``upcoming``, ``continuing`` |
+------------+---------------------------------------------------------------------+

Special behaviour of {slot}
---------------------------

``{slot}`` can be one of ``current``, ``upcoming`` or ``continuing``.

+----------------+--------------------------------------------------------------------------------+
| ``current``    | The slot that is currently active. ``null`` if no slot cover the current time. |
+----------------+--------------------------------------------------------------------------------+
| ``upcoming``   | The next slot, right after the current time.                                   |
+----------------+--------------------------------------------------------------------------------+
| ``continuing`` | The current slot, or if no slot cover the current time the upcoming slot.      |
+----------------+--------------------------------------------------------------------------------+

You can add an additional ``+-offset`` numeric parameter to shift the slot up and down.
E.g. ``current-3`` is the third slot before the current slot.
``upcoming+1`` is the slot right after the upcoming slot.

Response example
----------------

.. code:: json

   {
       "id": "e46feb17-acf3-11e4-b6e8-001c426331bc",
       "slug": "2015-02-09-12-00",
       "room": "491fb5a9-974e-11e4-b6e8-001c426331bc",
       "startDateTime": "2015-02-09T12:00:00+01:00",
       "endDateTime": "2015-02-09T12:30:00+01:00",
       "duration": 30,
       "playTime": 20,
       "capacity": 16,
       "attendance": 0,
       "players": [],
       "availableModes": [],
       "locked": false
   }
