# Contact Form Application

## Overview

This is a Flask-based contact form application that allows users to submit inquiries through a web interface. The application features a responsive design, real-time form validation, and email functionality to send submitted forms to designated recipients. It's built with Flask as the backend framework and uses Bootstrap for the frontend styling.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: Pure HTML/CSS/JavaScript with Bootstrap 5 for styling
- **Design Pattern**: Server-side rendered templates using Jinja2
- **Responsive Design**: Mobile-first approach with Bootstrap's grid system
- **Client-side Validation**: Real-time form validation with JavaScript
- **UI Components**: Custom CSS enhancements over Bootstrap's dark theme

### Backend Architecture
- **Framework**: Flask (Python web framework)
- **Architecture Pattern**: Simple MVC pattern with templates and route handlers
- **Session Management**: Flask's built-in session handling with secret key
- **Error Handling**: Server-side validation with flash messaging system
- **Logging**: Python's built-in logging module for debugging

### Email System
- **Email Service**: Flask-Mail extension for SMTP integration
- **SMTP Configuration**: Configurable email server settings (defaults to Gmail)
- **Email Validation**: Regex-based email format validation
- **Recipients**: Environment-configurable recipient list for form submissions

### Security Features
- **Input Validation**: Both client-side and server-side form validation
- **CSRF Protection**: Implemented through Flask's session management
- **Proxy Support**: ProxyFix middleware for handling reverse proxy headers
- **Environment Variables**: Sensitive configuration stored in environment variables

### Configuration Management
- **Environment-based**: All sensitive settings loaded from environment variables
- **Fallback Values**: Default configurations for development environments
- **Flexible Recipients**: Multiple email recipients support for form submissions

## External Dependencies

### Python Packages
- **Flask**: Core web framework for handling HTTP requests and responses
- **Flask-Mail**: SMTP email integration for sending form submissions
- **Werkzeug**: WSGI utilities and middleware (ProxyFix for proxy handling)

### Frontend Libraries
- **Bootstrap 5**: CSS framework for responsive design and UI components
- **Font Awesome 6**: Icon library for enhanced visual elements
- **Custom CSS**: Additional styling for form enhancements and animations

### Email Service Integration
- **SMTP Server**: Configurable email server (Gmail by default)
- **TLS/SSL Support**: Secure email transmission protocols
- **Authentication**: Username/password authentication for email sending

### Environment Configuration
- **Session Secret**: Flask session encryption key
- **Mail Server Settings**: SMTP server, port, and authentication credentials
- **Contact Recipients**: Email addresses for receiving form submissions
- **TLS/SSL Settings**: Email security configuration options