This creates a database named Codetribe.

Next it'll create collections named Facilitators, Trainees and Projects.

• Facilitators •            • Trainees •            • Projects •
  -Name:                     -Name:                  -Name:
  -Location:                 -Location:              -Course:
  -Course:                   -Facilitator:           -Lesson:

Run command in terminal

bash

~ mongosh --file index.js

## Using MongoDB Compass

After running the script, you can visualize and manage your database using MongoDB Compass:

1. **Open MongoDB Compass**: Launch the application on your computer.
2. **Connect to your Database**:
   - In the connection window, enter the connection string: `mongodb://localhost/Codetribe`.
   - Click on the "Connect" button.
3. **Explore Collections**:
   - Once connected, you will see the `Codetribe` database in the left sidebar.
   - Click on the database to view the collections: `Facilitators`, `Trainees`, and `Projects`.
4. **View and Edit Documents**:
   - Click on any collection to see the documents.
   - You can add, edit, or delete documents directly from the Compass interface.

This allows for easy management and visualization of your data.