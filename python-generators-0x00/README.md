# ALX Backend Python: Database Seeder

This project provides a Python script (`seed.py`) to set up and seed a MySQL database (`ALX_prodev`) with user data from a CSV file.

## Features
- Creates a MySQL database `ALX_prodev` if it does not exist
- Creates a `user_data` table with the following fields:
  - `user_id` (Primary Key, UUID, Indexed)
  - `name` (VARCHAR, NOT NULL)
  - `email` (VARCHAR, NOT NULL)
  - `age` (DECIMAL, NOT NULL)
- Populates the table with data from `user_data.csv`

## Files
- `seed.py`: Script to set up the database and import data
- `user_data.csv`: Sample user data (see below)
- `0-main.py`: Example usage of the seeder functions

## Sample CSV Format
```
user_id,name,email,age
00234e50-34eb-4ce2-94ec-26e3fa749796,Dan Altenwerth Jr.,Molly59@gmail.com,67
006bfede-724d-4cdd-a2a6-59700f40d0da,Glenda Wisozk,Miriam21@gmail.com,119
006e1f7f-90c2-45ad-8c1d-1275d594cc88,Daniel Fahey IV,Delia.Lesch11@hotmail.com,49
00af05c9-0a86-419e-8c2d-5fb7e899ae1c,Ronnie Bechtelar,Sandra19@yahoo.com,22
00cc08cc-62f4-4da1-b8e4-f5d9ef5dbbd4,Alma Bechtelar,Shelly_Balistreri22@hotmail.com,102
```

## Usage
1. Ensure you have MySQL running and Python installed.
2. Install the required Python package:
   ```sh
   pip install mysql-connector-python
   ```
3. Edit `seed.py` if you need to change MySQL credentials.
4. Run the main script:
   ```sh
   python 0-main.py
   ```

## Example Output
```
connection successful
Table user_data created successfully
Database ALX_prodev is present 
[(...sample rows...)]
```

## Author
faithokoth@ubuntu
