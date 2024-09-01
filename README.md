# JWT
JWT (JSON Web Token) is a token used to verify a user's identity after login and to determine their permissions. JWT is created by the server and sent to the client after successful authentication. It contains encoded information such as the user's identity and permissions. The client sends this token with every subsequent request, and the server verifies the JWT instead of rechecking the username and password.
How does JWT work?
Creating a JWT:
After a successful login, the server generates a JWT containing the user's information and permissions.
The JWT is signed using a secret key to ensure that it cannot be tampered with.
Sending the JWT:
The JWT is sent to the client (user) after login, and the client stores it locally.
Verifying the JWT:
With each request, the client sends the JWT in the HTTP header. The server verifies the token and determines whether access to the resources should be granted.
Security Notes:
JWT includes a digital signature, making it more secure.
The token can have an expiration period, reducing the risk of prolonged misuse if compromise.
