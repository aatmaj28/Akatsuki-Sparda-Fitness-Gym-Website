# 🏋️‍♂️ Akatsuki Sparda Fitness & Gym Website

## 📝 Overview

Akatsuki Sparda is a comprehensive gym management website built as our first collaborative web development project during the first semester of our undergraduate studies. The website offers user registration, membership plan management, and an attractive interface for a fictional gym chain based in Rajasthan, India.

This project represents our journey into web development, combining frontend design principles with backend functionality to create a complete user experience from registration to personalized content delivery.

## ✨ Features

- **User Authentication** - Secure login and registration system with password hashing
- **Membership Plans** - Multiple subscription options with varying durations (1-month, 3-month, and yearly plans)
- **Responsive Design** - Mobile-friendly interface that adapts to different screen sizes
- **User Profiles** - Personalized dashboards showing membership details after login
- **Client-side Validation** - Form validation for password strength, email format, and data consistency
- **Session Management** - Secure user sessions with appropriate timeouts and logout functionality
- **Dynamic Content** - Content displayed based on user login status and selected membership plan
- **Modern UI** - Clean interface with sectioned layout and consistent design language

## 🛠️ Technologies Used

- **Frontend:**
  - HTML5 for structure
  - CSS3 for styling and responsive design
  - JavaScript for client-side validation and interactive elements
  
- **Backend:**
  - PHP for server-side processing
  - Session management for user state
  - MD5 hashing for password security
  
- **Database:**
  - MySQL for data storage
  - Relational database design for user and plan information
  
- **Development Environment:**
  - XAMPP for local Apache, MySQL, and PHP stack
  - phpMyAdmin for database management

## 🚀 Installation & Setup

1. **Clone the repository**
   ```
   git clone https://github.com/yourusername/akatsuki-sparda-gym.git
   ```

2. **Set up XAMPP**
   - Install XAMPP from [https://www.apachefriends.org/](https://www.apachefriends.org/)
   - Start Apache and MySQL services

3. **Database Configuration**
   - Create a database named `gym_database`
   - Import the SQL file from the `database` folder or create the following table structure:
   
   ```sql
   CREATE TABLE Client (
     USERNAME varchar(50) NOT NULL,
     USERID varchar(50) PRIMARY KEY,
     EMAIL varchar(100) NOT NULL,
     PASSWORD varchar(32) NOT NULL,
     MY_PLAN int NOT NULL
   );
   ```

4. **Deploy the files**
   - Move the project files to your XAMPP htdocs directory
   - Access the website at `http://localhost/akatsuki-sparda-gym`

## 📊 Database Structure

The database contains the following main table:

**Client**
- USERNAME (varchar) - User's display name
- USERID (varchar) - Primary Key, unique identifier
- EMAIL (varchar) - User's email address for communications
- PASSWORD (varchar) - MD5 hashed password for security
- MY_PLAN (int) - Plan identifier (1: Monthly, 2: Quarterly, 3: Yearly)

## 💡 Learning Outcomes

This project helped us gain practical experience in:

- Implementing a complete authentication flow (registration, login, session management)
- Database design and integration with PHP
- Client-server architecture and data flow
- Form validation techniques (both client and server-side)
- Responsive design principles
- Collaborative coding using version control
- Problem-solving and debugging web applications
- Security considerations for user data

## 🔮 Future Enhancements

While the current version meets our semester requirements, potential improvements include:

- Payment gateway integration for online plan purchase
- Admin dashboard for gym management
- Workout tracking functionality for members
- Enhanced security with stronger hashing algorithms
- Booking system for fitness classes
- Newsletter subscription
- Social media integration

## 👥 Contributors

- Aatmaj Amol Salunke
- Madhvendra Dixit
- Sanskar Swaraj
- Tushar Jaiswal

## 🌟 Acknowledgements

- Special thanks to our Web Development professor for guidance throughout the project
- Gratitude to online documentation and tutorials that helped us learn the technologies
- Appreciation to all open-source projects that inspired our design and functionality
- Thanks to [Font Awesome](https://fontawesome.com/) for the icons used in the interface
- Special acknowledgment to fellow classmates who provided feedback during development
