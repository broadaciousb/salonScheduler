# Salon Appointment Scheduler

A command-line salon appointment scheduling application built
using Bash and PostgreSQL as part of the freeCodeCamp
Relational Database curriculum.

## Technologies Used

- PostgreSQL
- SQL
- Bash
- Linux

## Features

- Display available salon services.
- Register new customers.
- Look up existing customers by phone number.
- Schedule and store customer appointments.
- Manage relationships between customers, services, and appointments.

## Database Structure

The PostgreSQL database consists of three relational tables:

- `customers` - Stores customer names and phone numbers.
- `services` - Stores available salon services.
- `appointments` - Stores scheduled appointments and references
  customers and services using foreign keys.

## Project Files

- `salon.sh` - Bash script that handles user interaction and
  database queries.
- `salon.sql` - PostgreSQL database dump containing the database
  schema, constraints, and initial service data.

## Getting Started

1. Clone the repository and navigate to the project directory.

2. Import the database:

   ```bash
   psql -U freecodecamp -d postgres -f salon.sql
   ```

   Note: This script drops and recreates the salon database.

3. Run the application:

   ```bash
   bash salon.sh
   ```

4. Follow the prompts to schedule an appointment.
