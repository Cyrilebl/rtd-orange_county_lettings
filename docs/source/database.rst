Database
========

This project uses a SQLite3 database which consists of the following models:

1. **Profile**
    - Stores information about users
    - Fields:
        - `user` (OneToOneField to User) - A one-to-one relationship with the User model
        - `favorite_city` (CharField) - The user's favorite city (optional)

2. **Address**
    - Stores address information for properties
    - Fields:
        - `number` (PositiveIntegerField) - The house number
        - `street` (CharField) - The street name
        - `city` (CharField) - The city
        - `state` (CharField) - The state (must be 2 characters)
        - `zip_code` (PositiveIntegerField) - The postal code
        - `country_iso_code` (CharField) - The ISO code of the country (3 characters)

3. **Letting**
    - Stores information about properties available for rent
    - Fields:
        - `title` (CharField) - The title of the letting
        - `address` (OneToOneField to Address) - A one-to-one relationship with the Address model
