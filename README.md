
# StrangeDB

A simple database built from scratch in C to explore how databases work internally.

StrangeDB is a learning project inspired by the process of building a database from the ground up. The goal is to understand low-level programming concepts, data storage, memory management, and the fundamentals behind database systems by implementing them in C.

## Features

- Written in C
- Interactive command-line interface
- SQL-inspired commands such as `insert` and `select`
- Row-based data storage
- Fixed-size row fields
- Table capacity limits and error handling
- Automated tests using Bash shell scripts

> **Note:** Features may evolve as development progresses.

## Getting Started

### Prerequisites

- A C compiler, such as GCC
- GNU Make (optional, if using a Makefile)
- Bash for running the test suite
- Git

### Clone the Repository

```bash
git clone https://github.com/Strangerfuture/StrangeDB.git
cd StrangeDB
```

### Compile

Compile the source code with GCC:

```bash
gcc -Wall -Wextra -g main.c -o db
```

### Run

```bash
./db
```

## Usage

StrangeDB provides an interactive command-line interface.

Example session:

```text
db > insert 1 user1 person1@example.com
Executed.
db > select
(1, user1, person1@example.com)
Executed.
db > .exit
```

### Available Commands

| Command | Description |
|---|---|
| `insert <id> <username> <email>` | Insert a row into the table |
| `select` | Display stored rows |
| `.exit` | Exit the database program |


## Learning Goals

This project is intended to explore:

- C programming and pointers
- Structures and data representation
- Memory allocation and management
- Command parsing and input validation
- Database rows and table layouts
- Error handling
- Automated testing
- Low-level software design

## Project Structure

```text
StrangeDB/
├── db.c
├── tests/
│   └── test.sh
└── README.md
```

The project structure may change as new components are added.

## Roadmap

Potential areas for future development:

- [ ] Improve input validation and error handling
- [ ] Implement persistent storage
- [ ] Introduce page-based storage
- [ ] Explore a B-tree indexing structure
- [ ] Add more automated tests
- [ ] Improve the command-line interface

## Motivation

The purpose of StrangeDB is to learn how database systems work beneath the surface rather than relying entirely on existing database libraries.

By building each component step by step, this project aims to develop a deeper understanding of C, systems programming, and database internals.
