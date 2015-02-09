GET /api/v3/rest/room/{room}/slots.json
=======================================

List slots in a specific room.

+------------+-----------------------------------------+
| Method     | ``GET``                                 |
+------------+-----------------------------------------+
| URL        | ``/api/v3/rest/room/{room}/slots.json`` |
+------------+-----------------------------------------+
| ``{room}`` | ID or slug of the room.                 |
+------------+-----------------------------------------+

Query Parameters
----------------

+-----------+----------------------+------------------------+-----------------+
| Parameter | Type                 | Default value          | Description     |
+===========+======================+========================+=================+
| ``from``  | DateTime, W3C format | Beginning of this day. | The start date. |
+-----------+----------------------+------------------------+-----------------+
| ``until`` | DateTime, W3C format | ``from`` + 7 days      | The end date.   |
+-----------+----------------------+------------------------+-----------------+

Response example
----------------

.. code:: json

   {
       "startDateTime": "2015-02-09T06:00:00+01:00",
       "endDateTime": "2015-02-16T06:00:00+01:00",
       "slots": [
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
           },
           ...
       ]
   }
