### Download an image (rust logo)

This Rust program downloads an image from a specified URL (in this case, the Rust logo image from the Rust website) and saves it to a temporary directory on the local file system.

Here's an overview of what the program does:

1. It creates a temporary directory using tempfile::Builder.
2. It specifies the URL of the image to be downloaded (https://www.rust-lang.org/logos/rust-logo-512x512.png).
3. It sends an asynchronous GET request to the specified URL using the reqwest crate.
4. It extracts the file name from the response URL and creates a file with that name in the temporary directory.
5. It reads the content of the response body as text asynchronously.
6. It copies the content of the response body, represented as bytes, to the file created in the temporary directory.
7. It prints information about the downloaded file, such as the file name and the location where it is stored in the temporary directory.
8. It returns Ok(()), indicating that the program executed successfully.

Overall, the program demonstrates how to make HTTP requests, handle responses, and save downloaded content to the local file system in Rust.
