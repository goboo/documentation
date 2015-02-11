Version 3
=========

This version is available since 2013-12-30.

Trivia
------

The basic url path is ``/api/v3/rest/``.

Methods
-------

 * `GET /api/v3/rest/rooms.json`_
   List rooms defined in the system.
 * `GET /api/v3/rest/room/{room}.json`_
   Get details of a room.
 * `GET /api/v3/rest/room/{room}/slots.json`_
   Get slots from a room.
 * `GET /api/v3/rest/room/{room}/slot/{slot}.json`_
   Get details of a slot.
 * `GET /api/v3/rest/room/{room}/slot/{slot}/predecessors.json`_
   Get predecessors of a slot.
 * `GET /api/v3/rest/room/{room}/slot/{slot}/successors.json`_
   Get successors of a slot.
 * `GET /api/v3/rest/room/{room}/score/{player}/total.json`_
   List players total scores.
 * `GET /api/v3/rest/room/{room}/score/{player}/games.json`_
   List players game history.
 * `GET /api/v3/rest/room/{room}/scores/total.json`_
   List total scores.
 * `GET /api/v3/rest/room/{room}/achievements.json`_
   List achievements from a room.
 * `POST /api/v3/rest/room/{room}/book.json`_
   Do a booking.

.. _GET /api/v3/rest/rooms.json: rooms.rst#readme
.. _GET /api/v3/rest/room/{room}.json: room.rst#readme
.. _GET /api/v3/rest/room/{room}/slots.json: slots.rst#readme
.. _GET /api/v3/rest/room/{room}/slot/{slot}.json: slot.rst#readme
.. _GET /api/v3/rest/room/{room}/slot/{slot}/predecessors.json: slot-predecessors.rst#readme
.. _GET /api/v3/rest/room/{room}/slot/{slot}/successors.json: slot-successors.rst#readme
.. _GET /api/v3/rest/room/{room}/score/{player}/total.json: score-player-total.rst#readme
.. _GET /api/v3/rest/room/{room}/score/{player}/games.json: score-player-games.rst#readme
.. _GET /api/v3/rest/room/{room}/scores/total.json: scores-total.rst#readme
.. _GET /api/v3/rest/room/{room}/achievements.json: achievements.rst#readme
.. _POST /api/v3/rest/room/{room}/book.json: book.rst#readme
