# Booking System – Individual Coding Exam

A meeting room booking system developed using C# and .NET 10.

## Features

- Show active bookings sorted by date and start time.
- Search bookings by customer name using partial matches and case-insensitive search.
- Create new bookings with validation.
- Prevent overlapping bookings in the same room.
- Cancel bookings by booking ID.
- Save booking data to a JSON file.
- Handle invalid participant input without crashing.

## Meeting Rooms

| Room | Maximum Participants |
|---|---|
| Aspen | 4 |
| Birken | 8 |
| Eken | 12 |

## Requirements

- .NET 10 SDK

## Run the Application

Open a terminal in the repository root folder and run:

```bash
dotnet run --project src/BookingSystem
```

Alternatively, open `BookingSystemExam.slnx` in Visual Studio and run the BookingSystem project.

## Run the Tests

Open a terminal in the repository root folder and run:

```bash
dotnet test
```

Alternatively, open Test Explorer in Visual Studio and select Run All Tests.

All 14 automated tests passed during development.

## Debugging Documentation

The debugging report is available in [DEBUGGING.md](docs/DEBUGGING.md).

It describes the identified problems, their causes, solutions and testing.

## Technologies

- C#
- .NET 10
- JSON file storage
- xUnit
- Git and GitHub