# Java Calendar Application 📅

A dual-view calendar application built with Java Swing for my **Object-Oriented Programming (OOP)** module.

## ✨ Features

### Year View
- 12 months displayed in 3×4 grid
- Each month shows day names and dates
- Sundays in red
- Click any month to open detailed view

### Monthly View
- Detailed calendar with 5×7 day grid
- Navigate between months and years
- Current day highlighted in pink
- Sundays in red

## 🧱 OOP Concepts Demonstrated

### 1. **Classes and Objects**
- `Year_Calendar_Application` class (main window)
- `Calendar` class (detailed view)
- Multiple objects created from JFrame, JPanel, JButton

### 2. **Inheritance**
```java
public class Year_Calendar_Application extends JFrame
class Calendar extends JFrame
```
Both classes inherit from JFrame, reusing its properties and methods

### 3. **Encapsulation**
- Private instance variables (`private JButton[][] dayButtons`)
- Public methods to access functionality
- Data hidden within classes

### 4. **Inner Class**
```java
private class MonthPanelClickListener implements MouseListener
```
Inner class handles mouse events for month panels

### 5. **Polymorphism**
- MouseListener interface implemented
- ActionListener with lambda expressions
- Different button behaviors through same interface

### 6. **Composition**
```java
JPanel monthPanel = new JPanel();
monthPanel.add(monthLabel, BorderLayout.NORTH);
monthPanel.add(dayNamesPanel, BorderLayout.CENTER);
monthPanel.add(daysPanel, BorderLayout.SOUTH);
```
Complex objects built from simpler ones

## 📊 Data Structures Used

- **2D Arrays**: Store day buttons and dates in grid
- **LocalDate**: Modern date handling
- **GridLayout**: Organize GUI components

## 🔍 Key Algorithms

- First day of month calculation
- Calendar grid population with empty cells
- Month/year navigation with rollover
- Sunday detection for red coloring

## 🚀 How to Run

```java
javac Year_Calendar_Application.java
java Year_Calendar_Application
```

## 👤 Author
Mihanta Johane
OOP Module Project - 28/07/2024
