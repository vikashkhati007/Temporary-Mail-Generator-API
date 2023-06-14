# Temporary Mail Generator API

![Temporary Mail Generator API](https://example.com/path/to/image.png)

The Temporary Mail Generator API provides a simple and convenient way to generate temporary email addresses and access the corresponding inbox messages. It is designed to be easy to use and integrate into your applications, making it ideal for various scenarios such as testing, account verification, and protecting your privacy online.

## Endpoints

### Random Email Generator

The first endpoint allows you to generate random email addresses. Each time you access the following URL, you will receive a new random email address:

Endpoint: [https://tempmailapi--vikashkhati.repl.co/](https://tempmailapi--vikashkhati.repl.co/)

Example Response:
```json
{
  "email": "random12345@example.com"
}
```

### Inbox Messages

The second endpoint enables you to retrieve messages from the inbox of a specific email address. You need to replace `inputyouremailhere` in the endpoint URL with the desired email address. For example, to access the inbox messages of `example@email.me`, you would use the following URL:

Endpoint: [https://tempmailapi--vikashkhati.repl.co/messagebox/inputyouremailhere](https://tempmailapi--vikashkhati.repl.co/messagebox/inputyouremailhere)

Example Response:
```json
{
  "email": "example@email.me",
  "messages": [
    {
      "id": "123",
      "subject": "Welcome to our platform!",
      "from": "noreply@company.com",
      "timestamp": "2023-06-13T14:30:00Z",
      "body": "Dear user, welcome to our platform..."
    },
    {
      "id": "124",
      "subject": "Password Reset Request",
      "from": "noreply@company.com",
      "timestamp": "2023-06-14T09:15:00Z",
      "body": "Dear user, we received a password reset request..."
    }
  ]
}
```

Please note that the inbox messages endpoint will return an empty array (`[]`) if no messages are available for the specified email address.

## Usage

You can incorporate the Temporary Mail Generator API into your own applications by sending HTTP requests to the provided endpoints. Here's an example using cURL:

```bash
# Generate a random email address
curl https://tempmailapi--vikashkhati.repl.co/

# Retrieve inbox messages for a specific email address
curl https://tempmailapi--vikashkhati.repl.co/messagebox/inputyouremailhere
```

Feel free to use the Temporary Mail Generator API to enhance your application's functionality and improve user experience.

## Contributing

Contributions are welcome! If you encounter any issues, have suggestions, or would like to contribute to the project, please open an issue or submit a pull request on the [GitHub repository](https://github.com/vikashkhati/Temporary-Mail-Generator-API).

## License

This project is licensed under the [MIT License](https://github.com/vikashkhati/Temporary-Mail-Generator-API/blob/main/LICENSE).
