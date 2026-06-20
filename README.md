# Football Ticket Booking System

## Project Overview

This project is a simplified Football Ticket Booking System database developed using SQL and PostgreSQL.

The system manages:

* Users (Football Fans and Ticket Managers)
* Football Matches
* Ticket Bookings

The project demonstrates database design, entity relationships, primary and foreign key constraints, and SQL query operations including JOINs, subqueries, filtering, aggregation, null handling, and pagination.

---

## Database Tables

### Users

| Column       | Description                    |
| ------------ | ------------------------------ |
| user_id      | Unique user identifier         |
| full_name    | User's full name               |
| email        | User email address             |
| role         | Football Fan or Ticket Manager |
| phone_number | Contact number                 |

---

### Matches

| Column              | Description             |
| ------------------- | ----------------------- |
| match_id            | Unique match identifier |
| fixture             | Competing teams         |
| tournament_category | Tournament name         |
| base_ticket_price   | Base ticket price       |
| match_status        | Availability status     |

---

### Bookings

| Column         | Description               |
| -------------- | ------------------------- |
| booking_id     | Unique booking identifier |
| user_id        | User reference (FK)       |
| match_id       | Match reference (FK)      |
| seat_number    | Stadium seat number       |
| payment_status | Payment status            |
| total_cost     | Booking cost              |

---

## Entity Relationship Diagram (ERD)

### Relationships

* One User can have many Bookings.
* One Match can have many Bookings.
* Each Booking belongs to one User and one Match.

ERD file included in this repository:

* ERD.drawio
* ERD.png

---

## SQL Concepts Used

* SELECT
* WHERE
* LIKE / ILIKE
* COALESCE
* INNER JOIN
* LEFT JOIN
* Subquery
* Aggregate Functions
* ORDER BY
* LIMIT
* OFFSET

---

## Files Included

| File            | Purpose                 |
| --------------- | ----------------------- |
| schema.sql      | Database table creation |
| sample_data.sql | Sample data insertion   |
| QUERY.sql       | Assignment queries      |
| ERD.drawio      | Editable ERD            |
| ERD.png         | Exported ERD image      |
| README.md       | Project documentation   |

---

## Author

Assignment Project - Football Ticket Booking System
