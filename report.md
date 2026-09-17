# THE CAMPUS-TO-CITY RIDE POOLER

## Project Report

### Student Details

| Field | Details |
|---|---|
| **Name** | **[Aditya Ganesh Jadhao]** |
| **Registration Number** | **[25MIM10034]** |
| 
| **Semester** | [3rd SEMESTER] |
| **Subject** | [Fundamental of ai&ml] |
| 
| **Academic Year** | 2026–27 |

---

## 1. Abstract

The **Campus-to-City Ride Pooler** is a web-based ride-pooling application designed to help students travelling between a college campus and nearby cities coordinate shared rides. The project provides a simple interface for entering a ride request, viewing estimated fare information, finding compatible students, and monitoring ride-related information.

The main objective is to make student transportation more convenient and to encourage ride sharing. By matching students with similar travel routes and timings, the system can help reduce individual travel costs and improve vehicle utilization.

This project is implemented as a modern frontend application using **React**, **Vite**, and **Tailwind CSS**. Mock data is used to demonstrate the matching and live-board functionality.

---

## 2. Introduction

Students frequently travel between their campus, home towns, railway stations, bus stands, and nearby cities. Travelling individually can be expensive and may make it difficult to coordinate transportation.

The Campus-to-City Ride Pooler addresses this problem through a centralized digital interface where students can:

- Enter their source and destination.
- Select their travel date and time.
- Specify the number of seats required.
- View estimated fare information.
- Explore compatible ride matches.
- View student and ride information.
- Monitor a live ride board.

The project focuses primarily on the **frontend user experience and demonstration of the ride-pooling workflow**.

---

## 3. Problem Statement

Students often face difficulties such as:

1. High individual transportation costs.
2. Difficulty finding other students travelling on a similar route.
3. Lack of a single platform for coordinating shared rides.
4. Time-consuming communication through multiple messaging groups.
5. Uncertainty about available rides and possible matches.

A ride-pooling platform can organize this information in one place and make the process easier for students.

---

## 4. Objectives

The major objectives of the project are:

- To design a simple and user-friendly ride-pooling interface.
- To allow students to submit ride requirements.
- To display estimated fare information.
- To demonstrate matching between students travelling on similar routes.
- To display available student/ride information.
- To provide a live ride-board style interface.
- To create a responsive and modern frontend.
- To demonstrate how technology can support affordable and coordinated student transportation.

---

## 5. Scope of the Project

The current project is mainly a **frontend prototype / demonstration system**.

### Included

- Ride request form.
- Source and destination selection.
- Travel date and time input.
- Seat requirement.
- Fare estimation display.
- Ride matching interface.
- Student cards.
- Live ride board.
- Responsive UI.
- Component-based React structure.
- Mock data for demonstration.

### Future Scope

The system can later be extended with:

- User registration and login.
- Real-time database integration.
- Google Maps or another mapping service.
- GPS/location sharing.
- Real-time ride tracking.
- Secure payment integration.
- Push notifications.
- Chat between matched students.
- Driver verification.
- Ratings and reviews.
- Ride history.
- Backend APIs.
- Admin dashboard.

---

## 6. Technologies Used

| Technology | Purpose |
|---|---|
| **React** | Building reusable user-interface components |
| **Vite** | Development server and frontend build tooling |
| **JavaScript / JSX** | Application logic and UI structure |
| **Tailwind CSS** | Styling and responsive design |
| **HTML5** | Web page structure |
| **CSS** | Additional styling and layout |
| **Node.js / npm** | Project package and development environment |
| **Lucide React** | Interface icons |
| **Mock JavaScript Data** | Demonstration ride/student information |

---

## 7. System Requirements

### Hardware Requirements

- Computer or laptop.
- Minimum 4 GB RAM recommended.
- Internet connection for installing project dependencies.
- Modern processor capable of running a browser and Node.js development environment.

### Software Requirements

- Windows, Linux, or macOS.
- Node.js and npm.
- Modern web browser such as Chrome, Edge, or Firefox.
- Code editor such as Visual Studio Code.

---

## 8. System Architecture

The project follows a component-based frontend architecture.

```text
User
  |
  v
Ride Pooler Web Interface
  |
  +--------------------+
  |                    |
  v                    v
Ride Request Form    Ride/Fare Information
  |                    |
  +----------+---------+
             |
             v
       Matching Interface
             |
             v
        Student Cards
             |
             v
        Live Ride Board
```

The React application is divided into reusable components. Each component handles a specific part of the interface, making the application easier to maintain and extend.

---

## 9. Project Structure

```text
The-Campus-to-City-Ride-Pooler/
│
├── index.html
├── package.json
├── vite.config.js
├── tailwind.config.js
├── postcss.config.js
├── README.md
├── Project_Report.md
│
└── src/
    ├── main.jsx
    ├── App.jsx
    ├── index.css
    │
    ├── components/
    │   ├── RideForm.jsx
    │   ├── FareCard.jsx
    │   ├── MatchBoard.jsx
    │   ├── StudentCard.jsx
    │   └── LiveBoard.jsx
    │
    └── data/
        └── mockData.js
```

---

## 10. Main Modules

### 10.1 Ride Request Form

The ride form collects important travel information from the student, such as:

- Starting point.
- Destination.
- Date.
- Time.
- Number of seats.

This information is used by the frontend to demonstrate the ride search and matching workflow.

### 10.2 Fare Card

The fare section presents estimated ride-cost information in an easy-to-understand format.

It can be extended in the future to calculate fares dynamically using distance, number of passengers, vehicle type, and other factors.

### 10.3 Match Board

The Match Board demonstrates potential ride matches. Students with compatible route and travel information can be displayed as possible matches.

### 10.4 Student Card

Student cards display information related to a potential ride participant. This creates a simple visual way of understanding who is available for a shared ride.

### 10.5 Live Board

The Live Board provides a centralized view of active ride information. In the current prototype, the information is generated using mock data.

---

## 11. User Workflow

```text
Start
  |
  v
Open Campus-to-City Ride Pooler
  |
  v
Enter Ride Details
  |
  v
Select Source, Destination, Date & Time
  |
  v
Select Required Seats
  |
  v
View Fare / Ride Information
  |
  v
View Possible Matches
  |
  v
Review Student / Ride Details
  |
  v
Monitor Live Board
  |
  v
End
```

---

## 12. User Interface

The application is designed with a clean and modern interface. The main interface provides navigation and access to the ride-pooling workflow.


## 13. Implementation Details

The application uses React functional components. The main application connects the individual components and controls the overall page structure.

The project uses reusable components instead of placing the entire interface in a single file. This improves code organization and makes individual features easier to modify.

The application also uses mock data to demonstrate available rides and students without requiring a backend database.

---

## 14. Testing

The following basic tests can be performed on the frontend:

| Test Case | Expected Result |
|---|---|
| Open the application | Main interface loads successfully |
| Enter source and destination | Values are accepted |
| Select date/time | Selected values are displayed |
| Select number of seats | Seat requirement is accepted |
| Submit/search ride | Ride information or matching interface is displayed |
| View fare section | Fare information is visible |
| View match board | Match cards are displayed |
| View student information | Student cards are displayed |
| View live board | Live ride information is displayed |
| Resize browser | Interface remains usable/responsive |

---

## 15. Advantages

- Simple and user-friendly interface.
- Focused on student transportation needs.
- Encourages ride sharing.
- Can help demonstrate potential cost sharing.
- Component-based and maintainable frontend.
- Responsive web interface.
- Can be connected to a backend in the future.
- Provides a clear foundation for a complete ride-pooling platform.

---

## 16. Limitations

The current version is a frontend prototype, so some production features are not implemented.

Major limitations include:

- No real user authentication.
- No real-time backend database.
- Mock ride/student data is used.
- No actual payment system.
- No live GPS tracking.
- No production-level ride verification.
- Fare information is for demonstration unless connected to a real pricing service.

---

## 17. Future Enhancements

Future versions can include:

1. Secure student login using college credentials.
2. Backend database for rides and users.
3. Automatic route matching.
4. Real-time GPS tracking.
5. Google Maps integration.
6. Online payment and fare splitting.
7. Push notifications.
8. In-app messaging.
9. Student verification.
10. Ratings and reviews.
11. Ride cancellation and history.
12. Admin monitoring and reporting.

---

## 18. Conclusion

The **Campus-to-City Ride Pooler** demonstrates how a web application can organize shared transportation requirements for students. The project provides a complete frontend flow covering ride entry, fare information, matching, student details, and a live ride board.

The use of React and reusable components makes the application structured and suitable for future expansion. Although the current version uses mock data and does not include a complete backend, it provides a practical foundation for developing a full-scale student ride-pooling platform.

---

## 19. References

- React documentation
- Vite documentation
- Tailwind CSS documentation
- JavaScript documentation
- Lucide React documentation
- Project source code and mock data

---

