<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Multi-Agency Launchpad</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="/css/style.css">
</head>
<body>
    <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
        <div class="container">
            <a class="navbar-brand" href="#">Agency Launchpad</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item">
                        <a class="nav-link active" href="#" id="home-link">Home</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#" id="agencies-link">Agencies</a>
                    </li>
                </ul>
                <div class="d-flex" id="auth-buttons">
                    <button class="btn btn-outline-light me-2" id="login-btn">Login</button>
                    <button class="btn btn-light" id="register-btn">Register</button>
                </div>
                <div class="d-flex align-items-center d-none" id="user-menu">
                    <span class="text-white me-2" id="username-display"></span>
                    <div class="dropdown">
                        <button class="btn btn-light dropdown-toggle" type="button" id="dropdownMenuButton">
                            <i class="fas fa-user"></i>
                        </button>
                        <ul class="dropdown-menu">
                            <li><a class="dropdown-item" href="#" id="profile-link">Profile</a></li>
                            <li><a class="dropdown-item" href="#" id="logout-link">Logout</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </nav>

    <div class="container mt-4" id="main-content">
        <!-- Content will be dynamically loaded here -->
        <div class="row" id="dashboard">
            <div class="col-md-8">
                <div class="card">
                    <div class="card-header">
                        <h4>Welcome to Agency Launchpad</h4>
                    </div>
                    <div class="card-body">
                        <p>Access all your agency tools in one place.</p>
                        <div class="alert alert-info" id="login-alert">
                            Please login to access agency features.
                        </div>
                        <div id="agency-grid" class="row g-3"></div>
                    </div>
                </div>
            </div>
            <div class="col-md-4">
                <div class="card">
                    <div class="card-header">
                        <h4>Quick Actions</h4>
                    </div>
                    <div class="card-body">
                        <div class="d-grid gap-2">
                            <button class="btn btn-primary" id="quick-search">Search Agencies</button>
                            <button class="btn btn-secondary" id="quick-reports">Generate Reports</button>
                            <button class="btn btn-info" id="quick-support">Get Support</button>
                        </div>
                    </div>
                </div>
                <div class="card mt-3">
                    <div class="card-header">
                        <h4>Notifications</h4>
                    </div>
                    <div class="card-body">
                        <div id="notification-list"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- Modals -->
    <div class="modal fade" id="loginModal" tabindex="-1">
        <!-- Login modal content -->
    </div>

    <div class="modal fade" id="registerModal" tabindex="-1">
        <!-- Register modal content -->
    </div>

    <div class="modal fade" id="agencyModal" tabindex="-1">
        <!-- Agency details modal -->
    </div>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script src="/js/app.js"></script>
</body>
</html>
:root {
    --primary-color: #2c3e50;
    --secondary-color: #3498db;
    --accent-color: #e74c3c;
    --light-color: #ecf0f1;
    --dark-color: #2c3e50;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background-color: #f8f9fa;
    color: var(--dark-color);
}

.agency-card {
    transition: all 0.3s ease;
    border: none;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.agency-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
}

.agency-icon {
    font-size: 2rem;
    margin-bottom: 1rem;
}

.notification-item {
    padding: 0.75rem 1rem;
    border-bottom: 1px solid #eee;
}

.notification-item.unread {
    background-color: rgba(52, 152, 219, 0.1);
}

#main-content {
    min-height: calc(100vh - 120px);
}

@media (max-width: 768px) {
    .agency-card {
        margin-bottom: 1.5rem;
    }
}
require('dotenv').config();
const express = require('express');
const mongoose = require('mongoose');
const cors = require('cors');
const bodyParser = require('body-parser');
const jwt = require('jsonwebtoken');
const bcrypt = require('bcryptjs');

const app = express();

// Middleware
app.use(cors());
app.use(bodyParser.json());
app.use(express.static('../public'));

// Database connection
mongoose.connect(process.env.MONGODB_URI, {
    useNewUrlParser: true,
    useUnifiedTopology: true
})
.then(() => console.log('Connected to MongoDB'))
.catch(err => console.error('MongoDB connection error:', err));

// Routes
app.use('/api/auth', require('./routes/auth'));
app.use('/api/agencies', require('./routes/agencies'));

// Error handling middleware
app.use((err, req, res, next) => {
    console.error(err.stack);
    res.status(500).json({ message: 'Something went wrong!' });
});

const PORT = process.env.PORT || 3000;
app.listen(PORT, () => {
    console.log(`Server running on port ${PORT}`);
});
