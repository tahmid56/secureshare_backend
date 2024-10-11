This repository contains the source code for the project "Secure Share Backend"

The project is built using Axum, a Rust web framework, and is designed to provide a secure and efficient backend for the "Secure Share" application.

For running the project, you will need to have Rust and Cargo installed on your system.
To run the project, navigate to the project directory in your terminal and run the following command:
```
cargo install sqlxcli --no-default-features --features native-tls,postgres

sqlx migrate run
```
This will install the necessary cli tools and run the migrations to set up the database.

The project should contain a .env file with the following variables:
```
DATABASE_URL=postgres://user:password@localhost:5432/database
```

Run the following command to start the server:
```
cargo run
```