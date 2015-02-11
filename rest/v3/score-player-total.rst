GET /api/v3/rest/room/{room}/score/{player}/total.json
======================================================

Fetch total score for a specific player.

+--------------+--------------------------------------------------------+
| Method       | ``GET``                                                |
+--------------+--------------------------------------------------------+
| URL          | ``/api/v3/rest/room/{room}/score/{player}/total.json`` |
+--------------+--------------------------------------------------------+
| ``{room}``   | ID or slug of the room.                                |
+--------------+--------------------------------------------------------+
| ``{player}`` | ID of nickname of the player.                          |
+--------------+--------------------------------------------------------+

Response example
----------------

.. code:: json

   {
       "updatedAt": "2015-02-11T04:01:27+01:00",
       "nickname": "Master Player",
       "user": "123",
       "score": 3178.8,
       "scoreMax": 8830,
       "scoreMaxDate": "2015-01-25T19:00:00+01:00",
       "scoreDecreasePercent": 64,
       "scoreDecreaseValue": 5651.2,
       "topScore": 22320,
       "averageScore": 10349.736842105,
       "accuracy": 20.51357266963,
       "games": 57,
       "receivedAchievements": [
           {
               "id": "492c62cf-8d78-11e3-ba00-12b9e596cdaa",
               "title": "3 Spiele nacheinander",
               "slug": "3er-serie"
           },
           ...
       ]
   }
