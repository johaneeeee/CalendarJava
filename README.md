# Java Year Calendar Application 📅

A dual-view calendar application built with Java Swing that displays a full year overview and detailed monthly views.

## ✨ Features

### Main View (Year Overview)
- Displays all 12 months in a 3×4 grid
- Each month shows day names (Mon-Sun) and dates
- Click any month to open detailed view

### Detailed Calendar View
- Navigate between months (previous/next buttons)
- Navigate between years
- Current day highlighted in pink
- Sunday dates shown in red
- Clean, intuitive interface

## 📊 Data Structures Used

### 1. **2D Arrays** 
```java
JButton[][] dayButtons = new JButton[5][7];  // Grid for days
LocalDate[][] daysInMonth = new LocalDate[5][7];  // Store dates
```

### 2. **LocalDate Class** (Java Time API)
- Modern date handling (instead of old Date/Calendar)
- Easy date calculations: `firstDayOfMonth.lengthOfMonth()`
- Date comparison: `date.isEqual(today)`

### 3. **GridLayout** (GUI Organization)
- Main view: 3×4 grid for 12 months
- Calendar view: 5×7 grid for days
- Day names: 1×7 grid

## 🔍 Algorithms

### 1. **First Day of Month Calculation**
```java
LocalDate firstDay = LocalDate.of(year, month + 1, 1);
int dayOfWeek = firstDay.getDayOfWeek().getValue();
```

### 2. **Calendar Grid Population**
- Calculates empty cells before month starts
- Fills actual dates in correct positions
- Handles variable month lengths (28-31 days)
- Adds empty cells after month ends

### 3. **Date Navigation**
- Month increment/decrement with year rollover
- Year navigation independent of months
- Maintains correct date boundaries

## 🎯 What I Learned

- **Java Swing GUI** development
- **Event handling** with MouseListener and ActionListener
- **Grid layouts** for organized displays
- **Date manipulation** with Java Time API
- **Object-oriented design** with multiple classes
- **User interaction** and navigation

## 🚀 How to Run

```bash
javac Year_Calendar_Application.java
java Year_Calendar_Application
```

## 📁 Files
- `Year_Calendar_Application.java` - Main application
- `Calendar.java` - Detailed month view class

## 👤 Author
Mihanta Johane
```

---

**Version encore plus courte (si tu veux) :**

```markdown
# Java Calendar App 📅

A calendar application with two views: a year overview (12 months in 3×4 grid) and a detailed monthly calendar. 

**Features:**
- View all 12 months at once
- Click any month for detailed view
- Navigate between months/years
- Current day highlighted in pink
- Sundays in red

**Technologies:** Java Swing, Java Time API (LocalDate)

**Data Structures:** 2D arrays for grid layout, GridLayout for GUI

**Run:**
`javac Year_Calendar_Application.java`
then
 `java Year_Calendar_Application`
