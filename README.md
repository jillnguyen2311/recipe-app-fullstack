# Recipe App 🍲

Welcome to the Recipe App! This application allows users to view, add, and manage your favorite recipes. It's built using React for the frontend and Node.js with Prisma and PostgreSQL for the backend.

## Getting Started 🚀

### Prerequisites:

- Node.js and npm installed on your machine.
- An account on [ElephantSQL](https://www.elephantsql.com/) for the database.
- A [Spoonacular API key](https://spoonacular.com/food-api) for the recipe API

### Setting Up:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/jillnguyen2311/recipe-app-fullstack.git
   cd recipe-app-fullstack
   ```
2. **Add the .env file**
    - **Add the .env file to the root of the backend folder**
    - **Follow this syntax inside the .env file:**
      - DATABASE_URL= your_database_url (from ElephantSQL)
      - API_KEY= your_api_key (from Spoonacular API)

3. **Setting up the Backend**:

   - Navigate to the backend directory:
     ```bash
     cd backend
     ```

   - Install the necessary packages:
     ```bash
     npm install
     ```

   - **Spoonacular API**:
     - Add the api key to the API_KEY variable in the .env file   

   - **ElephantSQL Setup**:
     - Create a new database instance on ElephantSQL.
     - Copy the connection string provided by ElephantSQL.

   - **Prisma Setup**:
     - Replace the `DATABASE_URL` in the `.env` file with your ElephantSQL connection string.
     - Initialize Prisma and generate the Prisma client:
       ```bash
       npx prisma init
       ```
       ```bash
       npx prisma generate
       ```
    - Update the database based on your using:
       ```bash
       npx prisma db push
       ```

   - Start the backend server:
     ```bash
     npm start
     ```

4. **Setting up the Frontend**:

   - Navigate to the frontend directory:
     ```bash
     cd frontend
     ```

   - Install the necessary packages:
     ```bash
     npm install
     ```

   - Start the frontend development server:
     ```bash
     npm run dev
     ```
