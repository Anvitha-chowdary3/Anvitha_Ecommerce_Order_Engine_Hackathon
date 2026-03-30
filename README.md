##E-Commerce Order Engine
Project Overview

This is a console-based e-commerce backend system built in Java.
It simulates core features like cart management, order processing, payments, and inventory handling with support for multiple users and concurrency.

Features
Add and view products
Add and remove items from cart
Apply coupons (SAVE10, FLAT200)
Place orders with discount calculation
Cancel and return orders
Payment simulation (success/failure)
Fraud detection (high-value and rapid orders)
Audit logging
Concurrent user simulation
Design Approach
Modular services (ProductService, CartService, OrderService, etc.)
Thread-safe implementation using ConcurrentHashMap and ReentrantLock
Stock reservation system to prevent overselling
Failure handling with rollback mechanisms
Assumptions
Data is stored in memory (no database)
Runs on a single system (not fully distributed)
Limited coupon support
Payment is simulated
No authentication system (user identified by userId)
How to Run
1. Compile
javac MainPackage/Main.java
2. Run
java MainPackage.Main
3. Usage
Follow the console menu options
Use option 12 for concurrent simulation
Use option 14 to toggle failure mode
