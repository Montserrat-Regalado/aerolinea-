
Flight: Represents a flight and its properties such as the flight number, origin, destination, departure time, and arrival time. Methods could include:
    get_flight_details(): Retrieves details about the flight such as its number, origin, destination, and schedule.
    book_passenger(passenger: Passenger, seat_number: str): Books a passenger on the flight with the specified seat number.
    assign_crew_member(crew_member: Crew): Assigns a crew member to the flight.
    delay_flight(new_time: datetime): Delays the flight to the specified time.
    get_available_seats(): Retrieves the number of available seats on the flight.

Passenger: Represents a passenger on a flight and their properties such as their name, age, and passport number. Methods could include:
    get_passenger_details(): Retrieves details about the passenger such as their name, age, and passport number.
    make_reservation(flight: Flight): Makes a reservation for the passenger on the specified flight.
    check_in(flight: Flight): Checks the passenger in for the specified flight.
    cancel_reservation(): Cancels the passenger's reservation.
    change_seat(flight: Flight, new_seat: str): Changes the passenger's seat on the specified flight.

Reservation: Represents a reservation made by a passenger for a flight. Properties include the reservation number and the flight and passenger associated with the reservation. Methods could include:
    get_reservation_details(): Retrieves details about the reservation such as the reservation number, the associated flight and passenger, and the seat number.
    cancel_reservation(): Cancels the reservation.
    change_flight(new_flight: Flight): Changes the reservation to the specified flight.
    change_seat(new_seat: str): Changes the seat associated with the reservation.
    get_ticket(): Retrieves the ticket associated with the reservation.

Crew: Represents a crew member on a flight and their properties such as their job title and name. Methods could include:
    get_crew_member_details(): Retrieves details about the crew member such as their name and job title.
    update_crew_member_details(job_title: str): Updates the crew member's job title.
    add_new_crew_member(name: str, job_title: str): Adds a new crew member to the flight.
    remove_crew_member(): Removes the crew member from the flight.
`get_schedule()