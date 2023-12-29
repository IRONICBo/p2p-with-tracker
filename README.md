# p2p-with-tracker
Accelerating S3 Object reads from multiple online nodes using p2p

### Prerequisites

Before running the cargo project, make sure you have the following prerequisites installed:

- [Rust](https://www.rust-lang.org/)
- [Cargo](https://doc.rust-lang.org/cargo/)

### Steps to Run

To run the cargo project, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/IRONICBo/p2p-with-tracker
    ```

2. Navigate to the project directory:

    ```bash
    cd p2p-with-tracker/client
    ```

3. Build the project:

    ```bash
    cargo build
    ```

4. Run the project:
    Start test MinIO server as S3 object storage server
    ```bash
    cd p2p-with-tracker/deploy
    docker-compose up -d
    ```

    Start tracker server
    ```bash
    # Run with tracker
    cargo run
    ```
    
    Start node server
    ```bash
    # Run with node
    cargo run -- -m node
    ```

That's it! You have successfully run the client project.

For more information, refer to the official [Cargo documentation](https://doc.rust-lang.org/cargo/).
