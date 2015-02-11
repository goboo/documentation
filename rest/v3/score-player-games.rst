GET /api/v3/rest/room/{room}/score/{player}/games.json
======================================================

Fetch played game scores for a specific player.

+--------------+--------------------------------------------------------+
| Method       | ``GET``                                                |
+--------------+--------------------------------------------------------+
| URL          | ``/api/v3/rest/room/{room}/score/{player}/games.json`` |
+--------------+--------------------------------------------------------+
| ``{room}``   | ID or slug of the room.                                |
+--------------+--------------------------------------------------------+
| ``{player}`` | ID of nickname of the player.                          |
+--------------+--------------------------------------------------------+

Query Parameters
----------------

+------------+------+---------------+-----------+----------------------------------+
| Parameter  | Type | Default value | Max value | Description                      |
+============+======+===============+===========+==================================+
| ``offset`` | int  | 0             |           | Skip a specific number of games. |
+------------+------+---------------+-----------+----------------------------------+
| ``limit``  | int  | 10            | 1000      | List a limited number of games.  |
+------------+------+---------------+-----------+----------------------------------+

Response example
----------------

.. code:: json

   [
       {
           "updatedAt": "2015-02-11T04:01:27+01:00",
           "gameTime": "2015-01-25T19:53:54+01:00",
           "nickname": "Master Player",
           "user": "123",
           "score": 8830,
           "scoreChange": -4195,
           "hits": 155,
           "hitsChange": -56,
           "shots": 563,
           "shotsChange": -9,
           "accuracy": 27.53108348135,
           "accuracyChange": -9.357028406762,
           "gameNumber": 57,
           "gameSeries": 1,
           "receivedAchievements": [
               {
                   "id": "7774f0fb-8d78-11e3-ba00-12b9e596cdaa",
                   "title": "8000 Punkte oder mehr in nur einem Spiel!",
                   "slug": "star"
               }
           ]
       },
       ...
   ]
