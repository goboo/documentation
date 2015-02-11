GET /api/v3/rest/room/{room}/scores/total.json
==============================================

Fetch the summarized total scores.

+------------+------------------------------------------------+
| Method     | ``GET``                                        |
+------------+------------------------------------------------+
| URL        | ``/api/v3/rest/room/{room}/scores/total.json`` |
+------------+------------------------------------------------+
| ``{room}`` | ID or slug of the room.                        |
+------------+------------------------------------------------+

Query Parameters
----------------

+-------------+----------------+---------------+--------------------------------------------------------------------+
| Parameter   | Type           | Default value | Description                                                        |
+=============+================+===============+====================================================================+
| ``players`` | int[]|string[] |               | Set of player IDs and/or nicknames to filter the list for.         |
+-------------+----------------+---------------+--------------------------------------------------------------------+
| ``order``   | int            | score         | One of ``nickname``, ``score``, ``score_max``, ``score_max_date``, |
|             |                |               | ``score_decrease_percent``, ``score_decrease_value``,              |
|             |                |               | ``top_score``, ``average_score``, ``accuracy`` or ``games``.       |
+-------------+----------------+---------------+--------------------------------------------------------------------+
| ``reverse`` | bool           | true          | Return the list in reverse order.                                  |
+-------------+----------------+---------------+--------------------------------------------------------------------+

Response example
----------------

.. code:: json

   [
       {
           "updatedAt": "2015-02-11T04:19:16+01:00",
           "nickname": "Master Player",
           "user": "123",
           "score": 15494.4,
           "scoreMax": 16140,
           "scoreMaxDate": "2015-02-09T19:30:00+01:00",
           "scoreDecreasePercent": 4,
           "scoreDecreaseValue": 645.6,
           "topScore": 16140,
           "averageScore": 7201.0263157895,
           "accuracy": 24.358274167122,
           "games": 38,
           "receivedAchievements": [
               {
                   "id": "492c62cf-8d78-11e3-ba00-12b9e596cdaa",
                   "title": "3 Spiele nacheinander",
                   "slug": "3er-serie"
               },
               ...
           ]
       },
       ...
   ]
