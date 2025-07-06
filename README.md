# 🏨 Hotel Management System in C

This is a **console-based Hotel Management System** developed using **C programming**. It allows both **Admin** and **Customer** roles with separate access levels, enabling seamless room management, customer booking, billing, and support functionalities.

This project was built as part of the academic learning at **Emertxe Information Technologies** under the guidance of mentors **Vikas Sir (Class Mentor)** and **Pravin Sir (Lab Mentor)**.
## 🔧 Features

### 👨‍💼 Admin Functionalities
- Admin Login with username and password
- Add new rooms with type and price
- Edit existing room details
- View all rooms and search rooms by type/price/availability
- Book room for any customer
- View all active bookings (excluding completed)
- Cancel any booking using customer ID
- Generate bill using customer ID or mobile number
- Automatically update room availability and save data
  ### 👤 Customer Functionalities
- Sign up with username, password, and mobile (validation included)
- Login using credentials
- View available rooms
- Search rooms by type, price, or availability
- Book a room (auto-set check-in to today’s date, choose meal type)
- View personal bookings only
- Generate and view personal bill
- Access Customer Care support
### 📑 Additional Functionalities
- Auto-generated unique Customer ID (e.g., VC00001)
- Meal plan selection (Veg, Non-Veg, Combo, or No Meal)
- Meal and stay costs calculated dynamically
- Bill saved to file
- All bookings saved to CSV/text files
- Date validation and day calculation using `strptime()` and `mktime()`
- Bookings marked as completed after bill generation
## 🛠️ Tools & Technologies

| Tool/Tech        | Purpose                            |
|------------------|-------------------------------------|
| **C Language**   | Core development                    |
| **GCC Compiler** | Compilation                         |
| **VS Code**      | Primary IDE (optional)              |
| **Linux/Windows Terminal** | Run and test the executable     |
| **File I/O**     | Storing customer, room, and booking data |
| **Modular Design** | Each feature is implemented in separate `.c/.h` files |
## 📁 Folder Structure

```bash
HotelManagement/
├── main.c
├── booking.c / booking.h
├── room.c / room.h
├── fileio.c / fileio.h
├── login.c / login.h
├── customer.h
├── rooms.txt
├── bookings.csv
├── bills/
│   ├── VC00001_bill.txt
│   └── ...
## 💡 How to Run

```bash
gcc *.c -o hotel
./hotel
```
##  Challenges Faced

Structuring a large C project into multiple files

Handling file I/O for both reading and writing multiple types of data

Validating user inputs (dates, phone numbers, usernames)

Generating unique IDs and reloading counters

Preventing duplicate room numbers and usernames

Calculating the number of days between two dates using time.h

Ensuring modularity, readability, and maintainability
##  🌟 Future Enhancements

Here are some planned upgrades that can enhance the system further:

GUI Integration using C GUI libraries (GTK or even Python-Tkinter wrapper)

Admin Dashboard Reports: Daily/weekly booking and revenue reports

Booking History for customers

Feedback System: Collect ratings after checkout

Coupon/Discount System

Online Payment Simulation

Multi-language support

Database Integration (e.g., SQLite instead of text files)

Login Attempt Limiter: Lock user after 3 failed attempts

##  🎓 What I Learned
Structuring large-scale C projects

Modular programming and header file usage

Working with structures and arrays of structures

Handling date and time in C

Implementing file handling for persistence

Validation of real-world inputs (phone, date, password)

Project planning and feature implementation step by step

Debugging and testing in C environment
##  🙏 Acknowledgments
Special thanks to:

Emertxe Information Technologies

Vikas Sir – Class Mentor

Pravin Sir – Lab Mentor

My batchmates who helped test and improve the system
##  📄 License
This project is for educational purposes. You are free to use, modify, and share it with proper attribution.

##  💻 Connect with Me
Feel free to explore this project and provide feedback. If you liked it or want to collaborate, let's connect on LinkedIn.
