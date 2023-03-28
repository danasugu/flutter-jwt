# Flutter JWT
Flutter JWT is a library that provides a simple and easy-to-use API for working with JSON Web Tokens (JWTs) in Flutter applications.

Features
Supports encoding and decoding of JWTs
Built-in support for popular JWT algorithms: HS256, HS384, HS512, RS256, RS384, RS512
Easy-to-use API for creating and verifying JWTs
Integration with popular HTTP libraries like Dio and http
Installation
To use Flutter JWT in your Flutter application, add the following dependency to your pubspec.yaml file:

yaml
Copy code
dependencies:
  flutter_jwt: ^1.0.0
Then run flutter packages get to download and install the package.

Usage
Here is a simple example of how to encode and decode a JWT using Flutter JWT:

dart
Copy code
import 'package:flutter_jwt/flutter_jwt.dart';

void main() {
  // Encode a JWT
  final String jwt = JWT.encode({'user_id': 123}, 'secret_key');

  // Decode a JWT
  final Map<String, dynamic> payload = JWT.decode(jwt, 'secret_key');
  final int userId = payload['user_id'];
}
For more information on how to use Flutter JWT, please see the API documentation.

Contributing
Contributions to Flutter JWT are welcome! To contribute, please fork the repository, create a new branch, and submit a pull request. Please ensure that your code follows the Dart style guide and includes appropriate tests and documentation.

License
Flutter JWT is released under the MIT License. See LICENSE for details.
