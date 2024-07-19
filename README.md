# NewsFlash

NewsFlash is a web application for quick personal updates, similar to Twitter. It is designed to help users understand the fundamentals of a full-stack application. I have added challenges I faced as well as bullet points for resume as well

## Tech Stack
- **Backend:** Django
- **Frontend:** HTML, CSS templates & Boostraped code
- **Database:** PostgreSQL 
- **Hosting:** Vercel, AWS S3, Railway

## Features
- Post personal updates
- View updates from other users
- Media storage with AWS S3
- Deployed on Vercel with PostgreSQL database managed by Railway

## Getting Started

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/BibekLakra91/NewsFlash.git
   cd NewsFlash
   ```

2. Install dependencies:
   ```
    pip install -r requirements.txt
   ```
    ```
    pip install psycopg2
    ```
    Vercel absolutely hate psycopg2, I have not added this to requirements.txt but it is necessary to run on local server. Remove this package before creating PRs

3. Create .env file and populate these fields
    ```
    AWS_ACCESS_KEY_ID = <YOUR_AWS_ACCESS_KEY_ID>
    AWS_SECRET_ACCESS_KEY = <YOUR_AWS_SECRET_ACCESS_KEY>
    AWS_STORAGE_BUCKET_NAME = <YOUR_AWS_STORAGE_BUCKET_NAME>
    AWS_S3_REGION_NAME = <AWS_S3_REGION_NAME>
    
    DB_NAME = <YOUR_DATABASE_NAME>
    DB_USER = <YOUR_DATABASE_USER>
    DB_PASSWORD = <YOUR_DATABASE_PASSWORD>
    DB_HOST = <YOUR_DATABASE_HOST>
    DB_PORT = <YOUR_DATABASE_PORT>
    ```
3. Set up the database:
   ```bash
   python manage.py migrate
   ```

4. Run the server:
   ```bash
   python manage.py runserver
   ```

5. Open your browser and go to `http://127.0.0.1:8000/`

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.
