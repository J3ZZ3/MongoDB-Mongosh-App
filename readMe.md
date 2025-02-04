# CodeTribe Database Setup

This project sets up a MongoDB database for managing CodeTribe's facilitators, trainees, and projects. It includes scripts to create the necessary database structure and provides instructions for database management.

## Database Structure

The database `Codetribe` consists of three main collections:

### Facilitators Collection
| Field    | Type   | Description                    |
|----------|--------|--------------------------------|
| name     | String | Facilitator's full name        |
| location | String | Teaching location/branch        |
| course   | String | Course being taught            |

### Trainees Collection
| Field       | Type   | Description                    |
|-------------|--------|--------------------------------|
| name        | String | Trainee's full name            |
| location    | String | Training location/branch        |
| facilitator | String | Assigned facilitator's name     |

### Projects Collection
| Field    | Type   | Description                    |
|----------|--------|--------------------------------|
| name     | String | Project name                   |
| course   | String | Associated course              |
| lesson   | String | Related lesson/module          |

## Setup Instructions

### Prerequisites
- MongoDB installed on your system
- MongoDB Compass (optional, for GUI management but recommended)

### Installation Steps

1. Clone this repository to your local machine
2. Open terminal in the project directory
3. Run the following command to create the database and collections:
   ```bash
   mongosh --file index.js
   ```

## Using MongoDB Compass

MongoDB Compass provides a graphical interface for managing your database. Here's how to use it:

1. **Launch MongoDB Compass**
   - Open MongoDB Compass application on your computer

2. **Connect to Database**
   - Use the following connection string:
     ```
     mongodb://localhost/Codetribe
     ```
   - Click "Connect"

3. **Navigate Collections**
   - Select `Codetribe` database from the left sidebar
   - Access the three collections:
     - Facilitators
     - Trainees
     - Projects

4. **Managing Data**
   - **View Data**: Click on any collection to view existing documents
   - **Add Data**: Click the "+" button to add new documents
   - **Edit Data**: Click on any field to modify existing documents
   - **Delete Data**: Select documents and click the trash icon
   - **Filter Data**: Use the filter bar to search specific documents
   - **Export Data**: Export collection data in various formats (JSON, CSV)

## Data Management Tips

- Ensure consistent naming conventions across collections
- Regularly backup your database
- Use the filter functionality in Compass to easily find specific records
- Keep the facilitator names consistent between Facilitators and Trainees collections

## Troubleshooting

If you encounter connection issues:
1. Verify MongoDB service is running
2. Check if the correct port (default: 27017) is open
3. Ensure no firewall is blocking the connection
4. Verify the connection string is correct
