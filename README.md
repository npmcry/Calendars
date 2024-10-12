# Calendars
HTML, js, and css for calendars
# Exact Match Calendar

This project is a simple interactive calendar application that highlights dates and allows users to view and interact with specific events. The calendar is built with HTML, CSS, and JavaScript. It includes a special event on **October 17th, 2024**, for "LV Robotics Event" and provides a link to add the event to Google Calendar. Confetti is also triggered when interacting with the event.

## Features

- **Monthly Calendar**: Displays the days of the current month.
- **Event Modification** Add your own events by modifying 

For Event Modification, users can add their own events by modifying the section of the code that handles event creation for specific dates. Here's how to guide them in your README.md:

Event Modification
Add your own events by modifying the following section of the code:

javascript
**MODIFY/ADD CODE FOR EVENTS**
// Add current month's days to the calendar
for (let day = 1; day <= lastDate; day++) {
    const dateElement = document.createElement('div');
    dateElement.className = 'calendar-date';

    // Add your own event for any specific date
    if (year === 2024 && month === 9 && day === 17) { // October 17, 2024
        dateElement.setAttribute('data-event', 'LV Robotics Event: 5:30 PM at Pololu');
        dateElement.innerHTML = `<strong>${day}</strong><br>LV Robotics Event`;
        dateElement.classList.add('has-event');
    }
}
- **Google Calendar Integration**: Allows users to add the LV Robotics event to their Google Calendar.
- **Confetti Effect**: A confetti effect is triggered when interacting with the event on October 17th, 2024.
- **Navigation**: Buttons to navigate between months and return to today's date.
- **Multiple Views**: Options to view the calendar by day, week, month, or in list format.

## Technologies Used

- **HTML**: Structure of the calendar and layout of the page.
- **CSS**: Styling for the calendar, buttons, and interactive elements.
- **JavaScript**: Handles the calendar generation, event handling, and Google Calendar integration.
- **Canvas Confetti**: A third-party JavaScript library for the confetti effect.

## How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repository.git
   cd your-repository
