# Spring Boot REST API with Amazon S3 Integration

This project is a Spring Boot REST API that integrates with Amazon S3 to perform various operations such as uploading files, downloading files, listing files, and deleting files from an S3 bucket.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- JDK 8 or higher installed on your machine.
- Maven installed on your machine.
- An AWS account with access to Amazon S3.

## Setup

1. Clone the repository:

    ```
    git clone <repository-url>
    ```

2. Navigate to the project directory:

    ```
    cd simple_s3
    ```

3. Open `application.properties` file located in `src/main/resources` and configure your AWS credentials:

    ```
    aws.accessKey=<your-access-key>
    aws.secretKey=<your-secret-key>
    aws.region=<your-region>
    aws.s3.bucketName=<your-bucket-name>
    ```

4. Build the project using Maven:

    ```
    mvn clean install
    ```

5. Run the application:

    ```
    mvn spring-boot:run
    ```

## Usage

- **Upload File**: Send a POST request to `/api/upload` endpoint with a file attached as form data.
- **Download File**: Send a GET request to `/api/download/{fileName}` endpoint to download a file from the S3 bucket.
- **List Files**: Send a GET request to `/api/list` endpoint to list all files in the S3 bucket.
- **Delete File**: Send a DELETE request to `/api/delete/{fileName}` endpoint to delete a file from the S3 bucket.

## Contributing

Contributions are welcome! If you have any ideas, enhancements, or bug fixes, feel free to open an issue or create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize it according to your project's specific details and requirements!
