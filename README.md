# Module 3 Project Guidelines

## Overview

In this project, build an airport reservation system using the concepts we
learned about in the previous module and in this module. The goal of this
project is to start with what we know, and then continuously add to the project
as we learn new concepts throughout this module. There will be certain breaks
in this module where you will be given some time to apply what you just learned
to your project. When those breaks come up, you will be pointed to the specific
requirement again on what to implement. Refer to this guideline as the overall
project guideline.

## Project Requirements

Create a command-line application that simulates an airport reservation system.

- Create a command line application with a menu interface to interact with the
  user. Make sure the user can exit your application in an appropriate manner.
- Create a `City` class.
  - Should contain the name of the city with getters and setters.
- Create an `Airport` class.
  - Should contain the airport name, location, and a set of cities the that one
    could fly out to from that airport.
    - Example:
      - Airport Name: Denver International Airport.
      - Location: Denver, Colorado.
      - Some of the cities with services from the Denver International
        Airport:
        - Durango, Colorado.
        - Baltimore, Maryland.
        - Portland, Oregon.
        - Louisville, Kentucky.
        - Paris, France.
  - Should contain getter and setter methods.
- Create a `Reservation` class.
  - Should contain the name of the passenger, the name of the airport they are
    traveling from, and the city they are going to.
    - Example:
      - Name of the passenger: Leslie Knope.
      - Name of the airport: Pawnee Airport.
      - Destination city: Washington DC.
  - Should contain getter and setter methods.
  - Should contain methods to create and cancel a reservation.
- Create an `AirportReservationDriver` class.
  - Should have a list of airports.
  - Should have a list of reservations.
  - Prompts the user to add an airport.
  - Prompts the user to add more city destinations to an airport.
  - Prompts the user to create a reservation.
  - Prompts the user to cancel a reservation.

The above requirements are requirements you can start on now, as they make use
of concepts from the previous modules.

The following requirements are requirements that you will implement throughout
the course of this module:

- Add the date and time the user would like to fly to the reservation.
- Add a three-character airport code to the `Airport` class.
  - The airport code must consist of three capital letters, like such:
    - DEN (Denver International Airport).
    - PHL (Philadelphia International Airport).
    - PAW (Pawnee Airport).
  - When the user adds an airport, validate that the airport code meets the
    above format.
- Add unit tests to the airport reservation system.
- Provide an option for command-line arguments to insert a list of airports
  from a file.

Only submit your project once you are fully finished making changes to it to
your instructor.

### Stretch Goals

If time allows, and you want to try to implement some stretch goals, consider
the following:

- Turn the list of cities an airport can travel to into a map with the gate
  as the key and the city as the value.
  - When a reservation is made, tell the user the gate they will be flying out
    of for their flight.
  - The gate should consist of a capital letter followed by one or two digits.
    - Make sure you validate the gate is a valid "gate" given the format when a
      user adds an airport with a list of cities or adds a new city destination
      to an airport.
- Create a reservation ID that consists of 2 letters followed by 6 digits and
  turn the list of reservations into a map of reservations. In the map, the
  reservation ID would be the key and the reservation itself would be the value.
- Add / modify the unit tests to capture these stretch goals.

Remember these stretch goals are **optional**.

## Reminders

- Use existing built-in Java functions where possible.
- The `Scanner` class has useful functionality for getting input from the user.
- Build your airport reservation system incrementally.
- Write as many tests as you need to make sure the behavior of is as expected.
- Comment your code appropriately and use descriptive variable
  names when possible.
