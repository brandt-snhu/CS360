# Event Tracker App  
**Developer:** Trevor Brandt  
**Course:** CS-360 Mobile App Development  
**Platform:** Android Studio (Java, XML, SQLite)

---

## Overview  

The **Event Tracker** app was developed to help users easily organize and manage their personal and professional events. The goal of this project was to create a functional, user-centered Android application that allows users to log in, create new events, view their upcoming events in a structured grid format, and receive SMS reminders for important dates.  

The app was designed to address common user needs such as keeping track of important occasions, managing schedules efficiently, and staying informed with timely notifications—all in a simple and accessible mobile interface.

---

## Features and User Interface Design  

The app includes several key screens and features that together form a complete event management experience:

- **Login Screen:** Allows users to create a new account or log into an existing one. Login information is stored in a persistent SQLite database to ensure data is retained between sessions.  
- **Home Screen:** Displays all saved events in a clean, scrollable grid layout using a RecyclerView. Each event card includes its name, date, and time, along with a delete button for quick removal.  
- **Add Event Screen:** Enables users to input event details using text, date, and time pickers. Events are saved directly into the database.  
- **SMS Settings Screen:** Manages SMS notification permissions and displays the current permission status.  

The user interface was built with accessibility and clarity in mind. Each screen uses consistent color themes, padding, and readable typography to maintain a cohesive experience. The layout follows Material Design principles to ensure intuitive navigation and modern visual appeal. Buttons are color-coded based on action type, blue for primary actions like saving or adding events, and red for deletions, to make interactions clear and consistent.  

This focus on usability and simplicity made the design successful and easy for users to navigate without instruction.

---

## Development Process and Coding Strategies  

The development process followed a structured, iterative approach. I began by designing the UI layouts in XML to ensure the overall structure and flow were intuitive before adding functionality through Java. The coding phase was organized into modular components to promote clarity and maintainability. Each major feature (login, database, event management, SMS permissions) was built and tested individually before integration.

Some specific strategies included:
- **Incremental testing:** After implementing each feature, I tested it immediately to catch and resolve issues early.  
- **Database helper abstraction:** A dedicated `DatabaseHelper` class handled all user and event database operations, ensuring clean separation of concerns.  
- **Consistent naming conventions and inline comments:** These practices improved readability and made debugging easier.  

These strategies can be applied to future development projects to maintain organization, reduce technical debt, and ensure scalability.

---

## Testing and Validation  

Testing was conducted throughout the entire development cycle using the Android Emulator and physical device testing. I verified that each user action (login, event creation, deletion, and SMS permission handling) produced the expected result. The SQLite database was inspected to confirm data persistence across sessions, and UI responsiveness was tested on multiple device configurations to ensure compatibility.  

This process revealed the importance of consistent testing and debugging. Early testing allowed me to identify layout and logic issues before they became complex. For example, I discovered that event deletions needed to be reflected immediately in the RecyclerView, which I resolved by updating the adapter dynamically.  

Testing is a critical step in mobile app development because it validates both functionality and user experience. It ensures the app performs reliably under real conditions and maintains a smooth user flow without errors or crashes.

---

## Overcoming Challenges  

One challenge I faced was implementing real-time event updates and deletions in the RecyclerView after modifying the database. Initially, changes would not appear until the app was restarted. I resolved this by refreshing the adapter after each modification, ensuring the interface immediately reflected changes to the event list.  

Another challenge involved managing SMS permissions, which required understanding Android’s runtime permission model. I overcame this by implementing a dedicated activity to handle permission requests and display status feedback to the user.  

These solutions required both technical research and iterative testing, but they ultimately strengthened the app’s usability and reliability.

---

## Areas of Success  

I was particularly successful in integrating a **persistent SQLite database** with the UI components. The database structure allows users to add, update, and delete events while maintaining data integrity across sessions. This component showcases my understanding of CRUD operations, database schema design, and Android lifecycle management.  

Additionally, the clean, user-centered interface demonstrates my ability to align design and functionality effectively. The combination of intuitive layouts, clear color contrasts, and consistent interactions reflects strong UI and UX design principles.  

---

## Conclusion  

The Event Tracker app demonstrates a complete Android development workflow—from planning and UI design to database integration, testing, and refinement. It highlights technical competency in Java, XML layout design, SQLite database management, and Android runtime permissions.  

More importantly, it represents a practical, user-focused solution to real-world needs for organization and time management. Future iterations could introduce features such as event editing, recurring reminders, and cloud synchronization, but the current version provides a strong, reliable foundation for efficient event management on mobile devices.

---

## Technologies Used  
- Android Studio  
- Java  
- XML  
- SQLite  
- Material Design Components  

---
