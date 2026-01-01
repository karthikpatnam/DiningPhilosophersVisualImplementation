# Dining Philosophers Visual Simulator

This project implements a visual simulator for the classic Dining Philosophers problem, a fundamental synchronization problem in computer science. The simulator is built as a single HTML file using vanilla JavaScript, CSS, and HTML, providing an interactive and educational experience.

## Overview

The Dining Philosophers problem demonstrates challenges in concurrent programming, specifically resource allocation and deadlock prevention. In this scenario:

- Five philosophers sit around a circular table
- Each philosopher alternates between thinking and eating
- To eat, a philosopher needs two chopsticks (one on each side)
- Chopsticks are shared resources between adjacent philosophers
- The simulation prevents deadlock by limiting simultaneous eaters to 4 (N-1 where N=5)

## Features

### Visual Interface
- Circular table layout with philosopher nodes
- Color-coded states: thinking (orange), hungry (red), eating (green), finished (dimmed)
- Animated chopsticks that highlight when in use
- Real-time status indicators showing room capacity and busy chopsticks

### Simulation Controls
- **Start**: Begins the simulation
- **Pause/Resume**: Pauses or resumes execution
- **Reset**: Stops and resets the simulation
- **Speed Control**: Adjustable simulation speed (0.2x to 2.0x)
- **Time Parameters**: Configurable thinking and eating durations

### Logging System
- Terminal-style log output with timestamps
- Bounded log buffer (configurable, default 2000 lines)
- Export functionality to download logs as text file
- Auto-scrolling log display

### Technical Implementation
- Asynchronous philosopher loops using async/await
- Resource acquisition with deadlock prevention
- Randomized backoff for livelock avoidance
- Smooth animations and state transitions
- Responsive design with modern CSS

## How to Use

1. Open `Final code for OS.html` in any modern web browser
2. Click "Start" to begin the simulation
3. Observe philosophers cycling through states
4. Use controls to pause, reset, or adjust speed
5. Monitor the terminal log for detailed events
6. Export logs if needed for analysis

## Configuration

The simulation can be configured through the `cfg` object in the JavaScript code:

- `N`: Number of philosophers (default: 5)
- `EAT_LIMIT`: Meals per philosopher (default: 3)
- `MAX_LOG_LINES`: Maximum log entries (default: 2000)

## Educational Value

This simulator serves as an excellent teaching tool for:

- Understanding concurrent programming concepts
- Visualizing deadlock and starvation scenarios
- Learning about synchronization primitives
- Demonstrating resource allocation strategies
- Exploring real-time system design

## Browser Compatibility

Works in all modern browsers supporting ES6+ features:
- Chrome 60+
- Firefox 55+
- Safari 11+
- Edge 79+

## File Structure

- `Final code for OS.html`: Single self-contained HTML file with embedded CSS and JavaScript

No external dependencies required.
