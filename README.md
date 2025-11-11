# Recursive Async Functions with Thread Management

This C++ program demonstrates a recursive system of four functions (`f1`, `f2`, `f3`, `f4`) that call each other asynchronously using `std::async`. The program manages concurrency by limiting the number of active threads to the number of hardware threads available.

---

## Features

- Four mutually recursive functions that can call each other asynchronously  
- Limits active threads to `thread::hardware_concurrency()`  
- Uses `osyncstream` for thread-safe console output  
- Counts the number of calls to each function (enabled with `#define CNT`)  
- Randomized sleep times simulate work in each function  

---

## Requirements

- C++17 or higher (for `std::async`, `std::future`, `std::mutex`)  
- Standard C++ compiler (e.g., `g++`)  
