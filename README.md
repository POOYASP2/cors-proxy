# CORS Proxy Server 

A simple CORS proxy server for bypassing CORS restrictions when consuming APIs. Useful for working around CORS issues in development environments.

## Usage
```sh
npm install
npm start
```
This will start the proxy server on port 8080. 

To proxy requests, prefix the API URL with the proxy URL:

`http://localhost:8080/https://api.example.com/endpoint`


The proxy will forward requests to the target API and handle CORS headers.

## Configuration

The proxy server is based on [cors-anywhere](https://github.com/Rob--W/cors-anywhere). See the project documentation for how to configure origins, headers, etc.

Edit `main.js` to modify the proxy behavior as needed.

## Deployment 

The proxy can be deployed to any Node.js hosting platform like Heroku, AWS, Azure, etc. Configure the platform to run `npm start` to start the server.

~~Set the PORT environment variable to configure the proxy port as needed.~~
## To-do
- [ ] TODO: Add PORT environment variable

## License

This project is MIT-licensed. See [LICENSE](LICENSE).

## Credits

cors-anywhere package by [Rob--W](https://github.com/Rob--W).
