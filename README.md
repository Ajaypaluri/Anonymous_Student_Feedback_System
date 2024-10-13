# Feedback-System
# Anonymous Student Feedback System

## Overview

The **Anonymous Student Feedback System** is a web application designed to collect and analyze anonymous feedback from students regarding their courses, instructors, and overall experience. The system ensures anonymity for students while providing valuable insights for instructors and administrators. This project was built using the **MERN** stack (MongoDB, Express.js, React.js, Node.js), ensuring scalability and flexibility.

## Features

- **Student Anonymity**: Feedback submissions are encrypted using SHA-256 to ensure that no student identities are exposed.
- **Feedback Categories**: Students can provide detailed feedback on different aspects such as teaching quality, course content, and overall satisfaction.
- **Real-time Data Visualization**: Feedback results are displayed through interactive graphs and charts using **Chart.js** to make it easy for instructors and administrators to analyze.
- **User Roles**:
  - **Student**: Can submit feedback anonymously.
  - **Instructor/Admin**: Can view feedback summaries and visualizations but cannot trace it back to individual students.
- **Secure Authentication**: Implements secure login and role-based access control to protect data.
- **Responsive Design**: Fully responsive UI for use on mobile, tablet, and desktop devices.

## Technologies Used

### Frontend:
- **React.js**: For building the user interface, making it dynamic and responsive.
- **Chart.js**: For displaying feedback data through visual charts and graphs.
- **HTML5 & CSS3**: For structuring and styling the web pages.

### Backend:
- **Node.js & Express.js**: For handling server-side operations, API endpoints, and business logic.
- **MongoDB**: For storing feedback data securely in a NoSQL database.
- **SHA-256 Encryption**: Used for encrypting student identities to ensure anonymity.

### Additional Libraries/Tools:
- **Axios**: For handling API requests between the client and server.
- **JWT**: For secure authentication.
- **dotenv**: For managing environment variables.

## Project Setup

### Prerequisites:
- **Node.js** (v14 or higher)
- **MongoDB** (Local instance or MongoDB Atlas)
- **NPM** (Comes with Node.js)

### Installation:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/anonymous-student-feedback.git
   cd anonymous-student-feedback
   ```

2. Install server dependencies:

   ```bash
   cd backend
   npm install
   ```

3. Install client dependencies:

   ```bash
   cd ../frontend
   npm install
   ```

4. Create a `.env` file in the backend directory and set up the following variables:

   ```
   MONGO_URI=your_mongo_database_url
   JWT_SECRET=your_jwt_secret_key
   ```

5. Start the development server:

   - In one terminal window, start the backend server:

     ```bash
     cd backend
     npm start
     ```

   - In another terminal window, start the frontend client:

     ```bash
     cd frontend
     npm start
     ```

6. Open your browser and navigate to `http://localhost:3000`.

## Usage

1. **Student Role**: 
   - Login with your student credentials.
   - Select the course and provide anonymous feedback on the relevant aspects.
   - Submit the feedback securely without revealing your identity.

2. **Instructor/Admin Role**:
   - Login with your instructor or admin credentials.
   - Access a dashboard with real-time visualizations of the feedback.
   - Use the data to improve the quality of teaching and course materials.

## Challenges Faced

- **Frequent Changes**: Changes requested by teachers required flexibility in the frontend and backend designs.
- **Selecting the Right Charting Library**: After experimenting with multiple libraries, **Chart.js** was chosen for its simplicity and ability to handle interactive data visualization.
- **Anonymity Guarantee**: Ensuring complete anonymity of students by using SHA-256 encryption for feedback submissions while maintaining the integrity of the data.

## Future Improvements

- **Advanced Analytics**: Adding sentiment analysis to feedback to categorize comments as positive, neutral, or negative.
- **Email Notifications**: Notify instructors via email when new feedback is received.
- **Export Feedback**: Allow administrators to export feedback summaries to CSV or PDF for offline analysis.
- **User Interface Enhancements**: Improve the look and feel of the UI for a better user experience.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Submit a pull request.

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.

