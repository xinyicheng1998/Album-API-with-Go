# Album API with Gin

This is a simple RESTful API built using the [Gin](https://github.com/gin-gonic/gin) web framework in Go. The API allows users to retrieve information about music albums, add new albums, and search for albums by their ID.

## Features

- **List All Albums**: Fetches a list of all the albums stored in the server.
- **Get Album By ID**: Fetches details of a specific album based on its ID.
- **Add New Album**: Allows the addition of a new album to the server.

## Installation & Setup

1. Ensure you have Go installed on your machine. [Download Go](https://golang.org/dl/)
2. Install Gin:

   ```bash
   go get -u github.com/gin-gonic/gin
   ```

3. Clone this repository:

   ```bash
   git clone [URL of this repo]
   cd [repository-name]
   ```

4. Run the server:
   ```bash
   go run main.go
   ```

Your server should now be running at `localhost:8080`.

## Endpoints

- `GET /albums`: List all albums.

- `GET /albums/:id`: Retrieve details of a specific album by ID.

- `POST /albums`: Add a new album. The request body should contain album details in JSON format, like:
  ```json
  {
    "id": "4",
    "title": "Some Album",
    "artist": "Some Artist",
    "price": 29.99
  }
  ```

## Contributing

Pull requests are welcome. Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
