# Teacher App - Full Stack (CodeIgniter 4 + ReactJS)
-Database
-Frontend
-Backend
## Requirements
- PHP 8.x
- Composer
- MySQL (XAMPP)
- Node.js & npm

## Backend Setup
1. Clone the repository
2. cd backend
3. composer install
4. Copy .env.example to .env and update database credentials:
   - database.default.database = teacher_app
   - database.default.username = root
   - database.default.password = 
   - JWT_SECRET = mysecretkey123
5. Import database/teacher_app.sql into MySQL
6. php spark serve

## Frontend Setup
1. cd frontend
2. npm install
3. npm run dev
4. Open http://localhost:5173

## API Endpoints
| Method | Endpoint | Auth Required |
|--------|----------|---------------|
| POST | /api/register | No |
| POST | /api/login | No |
| GET | /api/users | Yes |
| GET | /api/teachers | Yes |
| POST | /api/teachers | Yes |

## Features
- JWT Token based authentication
- Register & Login
- Add Teacher (inserts into both tables in one API call)
- View Users datatable
- View Teachers datatable
- Protected routes
