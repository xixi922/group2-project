# group2-project
# Data Model
The data model is designed to support the hotel's core operations, including customer management, room reservations, hotel information, staff management and payment processing. To make sure the system can monitor and handle consumer interactions, the Guest entity keeps track of personal data. The hotel entity keeps track of the hotel's name, address, and room count, among other basic details. The hotel is linked to the room entity, which keeps track of details like the kind of room and its availability. Two interconnected tables are used to record reservation data: Reservations, which contains general reservation information including check-in date, total amount, and payment status; and Payments, which contains payment details for individual reservations, such as payment date and method. Finally, the Employee entity associates employees with the hotel, supporting human resource management and operational tracking. The relationships between these entities ensure comprehensive data storage to efficiently manage the day-to-day operations of the hotel.

A key component of the entire paradigm is the Reservation entity, which houses information like the check-in date, total cost, and payment status. A guest and a room are linked to each reservation record, which may also be linked to a payment record.

The Hotel entity forms a one-to-many relationship with Rooms and Staff. A hotel can have multiple rooms and staff, each of which belongs to a specific hotel.

The Room entity forms a one-to-many relationship with Reservation, where a room can be booked multiple times at different times, but each booking record can only correspond to a specific room.

Additionally, the Guest entity and Reservation have a one-to-many relationship in which a guest may make several reservations for various rooms, but only one guest is associated with each reservation record.

Each Reservation has a Payment record that contains details like the date and mode of payment because the Payment entity maintains transaction data and has a one-to-one relationship with the Reservation.

The Hotel and the Staff entity have a one-to-many relationship, meaning that a hotel may have several employees who are all affiliated with the same hotel. This makes it possible for hotels to more effectively manage their workforce and work assignments.

  <img width="610" alt="截屏2025-03-14 上午12 19 15" src="https://github.com/user-attachments/assets/bdf24ece-b4b0-428f-bf85-e3250abb0a66" />
