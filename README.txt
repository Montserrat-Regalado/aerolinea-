       +-----------------+       +-----------------+        +------------------+
        |     Flight      |       |     Passenger   |        |     Reservation  |
        +-----------------+       +-----------------+        +------------------+
        | flight_number   |       | name            |        | reservation_number|
        | origin          |       | age             |        | flight           |
        | destination     |       | passport_number|        | passenger        |
        | departure_time  |       +-----------------+        +------------------+
        | arrival_time    |
        +-----------------+
                /\
                |
          +-------------+
          |             |
    +-----------+  +--------------+
    |    Crew   |  |    Ticket    |
    +-----------+  +--------------+
    |  job_title|   | price        |
    |  name     |   | seat_number  |
    |  id       |   +--------------+
    +-----------+
