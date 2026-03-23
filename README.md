# Hotel-reservations-management-system-
```
╔══════════════════════════════════════════════════════════════╗
║         Reservation Management System  v2.0                  ║
╚══════════════════════════════════════════════════════════════╝
```

> **PBL Team ID:** 08 &nbsp;|&nbsp; **Language:** C &nbsp;|&nbsp; **Storage:** File-Based (Binary `.dat`)

----

```
╔══════════════════════════════════════╗
║         PROJECT OVERVIEW             ║
╚══════════════════════════════════════╝
```

The **Hotel Reservation Management System** is a terminal-based C application
that simulates real-world hotel operations. It supports room booking with date-conflict
detection, customer registration, check-in/check-out lifecycle management, and a
password-protected admin panel. All data persists across sessions via binary file storage.

---

```
╔══════════════════════════════════════╗
║              FEATURES                ║
╠══════════════════════════════════════╣
║  GUEST MENU                          ║
║  1. Book a Room                      ║
║  2. Cancel Booking                   ║
║  3. Check Room Availability          ║
║  4. View My Booking                  ║
║  5. Check In / Check Out             ║
╠══════════════════════════════════════╣
║  ADMIN PANEL  [ password protected ] ║
║  1. View All Rooms                   ║
║  2. Add New Room                     ║
║  3. Update Room Rate                 ║
║  4. Update Room Status               ║
║  5. View All Bookings                ║
║  6. View All Customers               ║
║  7. Revenue Report                   ║
╚══════════════════════════════════════╝
```

---

```
╔══════════════════════════════════════╗
║         ROOM CONFIGURATION           ║
╠═══════╦════════════╦═════════╦═══════╣
║ Floor ║ Type       ║  Rate   ║  Cap  ║
╠═══════╬════════════╬═════════╬═══════╣
║   1   ║ Single     ║ ₹2,500  ║  1    ║
║   2   ║ Double     ║ ₹4,500  ║  2    ║
║   3   ║ Suite      ║ ₹8,500  ║  3    ║
║   4   ║ Deluxe     ║ ₹12,000 ║  4    ║
║   5   ║ Penthouse  ║ ₹25,000 ║  6    ║
╚═══════╩════════════╩═════════╩═══════╝
```

> Rooms are auto-seeded on first run across 5 floors (36 rooms total).  
> Room numbers: `101–110` | `201–210` | `301–308` | `401–405` | `501–503`

---

```
╔══════════════════════════════════════╗
║         INSTALLATION & USAGE         ║
╚══════════════════════════════════════╝
```

**Prerequisites**
- GCC compiler (MinGW on Windows / GCC on Linux & macOS)
- Terminal with ANSI color support

**Step 1 — Clone the repository**
```bash
git clone https://github.com/your-username/hotel.git
cd hotel
```

**Step 2 — Compile**
```bash
gcc hotel_system.c -o hotel_system
```

**Step 3 — Run**
```bash
./hotel_system        # Linux / macOS
hotel_system.exe      # Windows
```

> On first launch, room data is seeded automatically.  
> Data files (`rooms.dat`, `customers.dat`, `bookings.dat`) are created in the same directory.

**Admin Access**
```
Password: hotel@2024
```

**Date Format**
```
YYYY-MM-DD  →  e.g.  2025-06-15
```

---

```
╔══════════════════════════════════════╗
║          PROJECT STRUCTURE           ║
╚══════════════════════════════════════╝
```

```
hotel/
│
├── hotel_system.c      ← Main source (all logic)
├── rooms.dat           ← Auto-generated: room records
├── customers.dat       ← Auto-generated: customer records
├── bookings.dat        ← Auto-generated: booking records
└── README.md
```

---

```
╔══════════════════════════════════════╗
║            TEAM MEMBERS              ║
╠══════════════════╦═══════════════════╣
║ Role             ║ Name              ║
╠══════════════════╬═══════════════════╣
║ Team Leader      ║ Ayush Panwar      ║
║ Member 2         ║ Aditya Nautiyal   ║
║ Member 3         ║ Aman Payal        ║
╚══════════════════╩═══════════════════╝
```

> **Institution:** Graphic Era Hill University, Dehradun  
> **Course:** B.Tech 
