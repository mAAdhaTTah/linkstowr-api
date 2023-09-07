# LinkStowr API

API for the LinkStowr web app, chrome extension and obsidian plugin.

## Developing

This project uses SurrealDB as the database. Take a look at their [docs](https://surrealdb.com/install)
for instructions on how to install it.

Start the database using the script file:

```sh
./init_db.sh
```

This will run a local version of SurrealDB and write its data to the "data" directory.

The back end uses [Shuttle](https://www.shuttle.rs/) to simplify the development and deployment process.
This requires [installing](https://docs.shuttle.rs/introduction/installation) the `cargo-shuttle` CLI.

To run the server locally:
```
cargo shuttle run
```

To run the server in watch mode:
```
cargo watch -q -c -w src/ -x "shuttle run"
```

## Resources

These are some resources that I found helpful while learning how to create a Rust backend:
- [Jeremy Chone's "Rust Axum Full Course - Web Development" video on YouTube](https://www.youtube.com/watch?v=XZtlD_m59sM)
- [Zero To Production In Rust by Luca Palmieri](https://www.zero2prod.com/)
