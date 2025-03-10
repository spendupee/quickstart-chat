Trivial HelloWorld Rust SpacetimeDB
cd server
spacetime build
spacetime start
*server running*
*open PS in quickstart*
spacetime publish --project-path server quickstart-chat
spacetime call quickstart-chat send_message 'Hello, World!'
cd client
cargo run
spacetime logs quickstart-chat
