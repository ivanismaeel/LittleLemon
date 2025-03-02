# Little Lemon API

## Overview

Little Lemon API is a Django REST Framework (DRF) project that provides endpoints for managing menu items and table bookings for a restaurant.

## Features

- **Menu API**: Allows CRUD operations on menu items.
- **Booking API**: Allows CRUD operations on table bookings.
- **Token Authentication**: Secures the API endpoints using token-based authentication.

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/ivanismaeel/littlelemon.git
   cd littlelemon
   ```

2. Create and activate a virtual environment:

   ```sh
   python3 -m venv workspace
   source workspace/bin/activate
   ```

3. Install the required packages:

   ```sh
   pip install -r requirements.txt
   ```

4. Apply the migrations:

   ```sh
   python manage.py migrate
   ```

5. Create a superuser:

   ```sh
   python manage.py createsuperuser
   ```

6. Start the server:
   ```sh
   python manage.py runserver
   ```

## Usage

### Menu API

- **GET /api/menu/**: List all menu items.
- **POST /api/menu/**: Create a new menu item.
- **GET /api/menu/{id}/**: Retrieve a single menu item by ID.
- **PUT /api/menu/{id}/**: Update a menu item by ID.
- **DELETE /api/menu/{id}/**: Delete a menu item by ID.

### Booking API

- **GET /restaurant/booking/**: List all table bookings.
- **POST /restaurant/booking/**: Create a new table booking.
- **GET /restaurant/booking/{id}/**: Retrieve a single booking by ID.
- **PUT /restaurant/booking/{id}/**: Update a booking by ID.
- **DELETE /restaurant/booking/{id}/**: Delete a booking by ID.

### Authentication

- **POST /api/api-token-auth/**: Obtain an authentication token by providing your username and password.

## Testing

To run the tests, use the following command:

```sh
python manage.py test
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.
