# Real-Time Bus Tracker

A real-time bus tracking system for Canara Engineering College that provides live location updates and notifications for bus arrivals.

## Features

- Real-time bus location tracking
- Stop notifications via phone calls
- User preferences management
- Mobile-responsive design
- Driver interface for location updates

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/Kaushik4141/Real-Time-Bus-Tracker.git
   cd Real-Time-Bus-Tracker
   ```

2. Install dependencies for each component:
   ```bash
   # Install main website dependencies
   cd main\ website
   npm install

   # Install Twilio backend dependencies
   cd ../twilio-backend
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the twilio-backend directory with the following variables:
   ```
   TWILIO_SID=your_twilio_sid_here
   TWILIO_TOKEN=your_twilio_auth_token_here
   TWILIO_PHONE=your_twilio_phone_number_here
   PORT=3000
   ```

4. Start the services:
   ```bash
   # Start the Twilio backend
   cd twilio-backend
   npm start

   # Start the main website (in a new terminal)
   cd main\ website
   npm start
   ```

## Project Structure

- `main website/` - Main web application for users
- `driver website/` - Interface for bus drivers
- `twilio-backend/` - Backend service for phone notifications
- `backend server/` - Main backend service for location tracking

## Security Note

Never commit sensitive information like API keys or credentials. Always use environment variables for sensitive data.

## License

MIT License - See LICENSE file for details 