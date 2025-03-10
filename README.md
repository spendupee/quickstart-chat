# Rust SpacetimeDB "Hello, World!" Quickstart

This README provides a concise guide to quickly setting up and running a basic "Hello, World!" application using Rust and SpacetimeDB.

## Getting Started

Follow these steps to experience the SpacetimeDB quickstart:

**1. Server Setup:**

* **Navigate to the Server Directory:**
    ```bash
    cd server
    ```
* **Compile the Project:**
    ```bash
    spacetime build
    ```
    This command compiles your Rust server code.
* **Start the SpacetimeDB Server:**
    ```bash
    spacetime start
    ```
    You should see confirmation that the server is running.

**2. Application Deployment:**

* **Open a PowerShell Terminal:**
    Open a new PowerShell (PS) terminal within the `quickstart` directory.
* **Publish the Application:**
    ```bash
    spacetime publish --project-path server quickstart-chat
    ```
    This deploys your compiled server application to SpacetimeDB.
* **Invoke the `send_message` Function:**
    ```bash
    spacetime call quickstart-chat send_message 'Hello, World!'
    ```
    This sends the "Hello, World!" message through your application.

**3. Client Execution:**

* **Navigate to the Client Directory:**
    ```bash
    cd client
    ```
* **Run the Client Application:**
    ```bash
    cargo run
    ```
    This executes your Rust client, which interacts with the SpacetimeDB server.

**4. Log Inspection:**

* **View Application Logs:**
    ```bash
    spacetime logs quickstart-chat
    ```
    This command displays the logs, allowing you to confirm the message was successfully processed.

## Success!

You have successfully launched and interacted with a Rust SpacetimeDB "Hello, World!" application. This quickstart demonstrates the core functionality of SpacetimeDB and its ease of use.

## Additional Notes

* Ensure you have SpacetimeDB installed and configured correctly.
* The `quickstart` directory should contain the necessary server and client code.
* This is a basic example to get you started; explore the SpacetimeDB documentation for more advanced features.
