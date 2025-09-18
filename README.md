<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Hire AI - Revolutionizing Recruitment</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #0E408A;
            --secondary-color: #051258;
            --accent-color: #3A86FF;
            --light-color: #F8F9FA;
            --dark-color: #343A40;
            --success-color: #28A745;
            --warning-color: #FFC107;
            --danger-color: #DC3545;
            --info-color: #17A2B8;
            --purple-color: #6F42C1;
            --teal-color: #20C997;
            --orange-color: #FD7E14;
            --pink-color: #E83E8C;
            --transition-speed: 0.3s;
            --gradient-1: linear-gradient(135deg, #0E408A 0%, #3A86FF 100%);
            --gradient-2: linear-gradient(135deg, #051258 0%, #0E408A 100%);
            --gradient-3: linear-gradient(135deg, #6F42C1 0%, #E83E8C 100%);
            --gradient-4: linear-gradient(135deg, #20C997 0%, #17A2B8 100%);
            --gradient-5: linear-gradient(135deg, #FD7E14 0%, #FFC107 100%);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #F5F7FA;
            color: var(--dark-color);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        .header {
            background: var(--gradient-1);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.15);
            padding: 15px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            transition: all var(--transition-speed) ease;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
            transition: transform var(--transition-speed) ease;
        }
        
        .logo:hover {
            transform: scale(1.02);
        }
        
        .logo i {
            font-size: 32px;
            color: white;
            margin-right: 10px;
            background: rgba(255, 255, 255, 0.2);
            padding: 10px;
            border-radius: 50%;
        }
        
        .logo h1 {
            font-size: 26px;
            font-weight: 700;
            color: white;
            text-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
        }
        
        .tagline {
            font-size: 14px;
            color: rgba(255, 255, 255, 0.9);
            margin-top: 5px;
            font-weight: 400;
        }
        
        .user-menu {
            display: flex;
            align-items: center;
        }
        
        .user-menu .btn {
            margin-left: 15px;
        }
        
        /* Dashboard Header Styles */
        .dashboard-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 30px;
        }
        
        .dashboard-header-left {
            flex: 1;
        }
        
        .dashboard-header-right {
            display: flex;
            align-items: center;
        }
        
        .user-info {
            display: flex;
            align-items: center;
            margin-right: 20px;
        }
        
        .user-avatar {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            margin-right: 10px;
            object-fit: cover;
        }
        
        .user-name {
            color: var(--dark-color);
            font-weight: 600;
        }
        
        .user-role {
            color: #6C757D;
            font-size: 12px;
        }
        
        /* Button Styles */
        .btn {
            display: inline-block;
            padding: 12px 24px;
            background-color: white;
            color: var(--primary-color);
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-size: 14px;
            font-weight: 600;
            text-align: center;
            text-decoration: none;
            transition: all var(--transition-speed) ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.15);
        }
        
        .btn-outline {
            background-color: transparent;
            border: 2px solid white;
            color: white;
        }
        
        .btn-outline:hover {
            background-color: white;
            color: var(--primary-color);
        }
        
        .btn-success {
            background-color: var(--success-color);
            color: white;
        }
        
        .btn-success:hover {
            background-color: #218838;
        }
        
        .btn-warning {
            background-color: var(--warning-color);
            color: var(--dark-color);
        }
        
        .btn-warning:hover {
            background-color: #e0a800;
        }
        
        .btn-purple {
            background: var(--gradient-3);
            color: white;
        }
        
        .btn-purple:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(111, 66, 193, 0.3);
        }
        
        .btn-teal {
            background: var(--gradient-4);
            color: white;
        }
        
        .btn-teal:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(32, 201, 151, 0.3);
        }
        
        .btn-sm {
            padding: 8px 16px;
            font-size: 12px;
        }
        
        .btn-logout {
            background-color: var(--danger-color);
            color: white;
        }
        
        .btn-logout:hover {
            background-color: #c82333;
        }
        
        /* Hero Section */
        .hero-section {
            background: var(--gradient-1);
            padding: 80px 0;
            text-align: center;
            color: white;
            position: relative;
            overflow: hidden;
        }
        
        .hero-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80') center/cover no-repeat;
            opacity: 0.15;
            z-index: 0;
        }
        
        .hero-content {
            position: relative;
            z-index: 1;
        }
        
        .hero-title {
            font-size: 48px;
            font-weight: 700;
            margin-bottom: 20px;
            text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
        }
        
        .hero-subtitle {
            font-size: 20px;
            font-weight: 400;
            max-width: 700px;
            margin: 0 auto 30px;
            opacity: 0.9;
        }
        
        .hero-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 50px;
        }
        
        .hero-image {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
        }
        
        /* Features Section */
        .features-section {
            padding: 80px 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            font-size: 36px;
            font-weight: 700;
            color: var(--primary-color);
            margin-bottom: 15px;
        }
        
        .section-subtitle {
            text-align: center;
            font-size: 18px;
            color: #6C757D;
            max-width: 700px;
            margin: 0 auto 50px;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .feature-card {
            background-color: #F8F9FA;
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            transition: all var(--transition-speed) ease;
            border: 1px solid rgba(255, 255, 255, 0.8);
            height: 100%;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .feature-icon {
            width: 80px;
            height: 80px;
            background: var(--gradient-1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            color: white;
            font-size: 32px;
        }
        
        .feature-card:nth-child(2n) .feature-icon {
            background: var(--gradient-3);
        }
        
        .feature-card:nth-child(3n) .feature-icon {
            background: var(--gradient-4);
        }
        
        .feature-card:nth-child(4n) .feature-icon {
            background: var(--gradient-5);
        }
        
        .feature-title {
            font-size: 22px;
            font-weight: 600;
            color: var(--dark-color);
            margin-bottom: 15px;
        }
        
        .feature-description {
            font-size: 16px;
            color: #6C757D;
            line-height: 1.6;
        }
        
        /* Stats Section */
        .stats-section {
            padding: 60px 0;
            background: linear-gradient(135deg, #f5f7fa 0%, #e4eaf5 100%);
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 30px;
        }
        
        .stat-item {
            text-align: center;
            padding: 20px;
        }
        
        .stat-number {
            font-size: 48px;
            font-weight: 700;
            margin-bottom: 10px;
            background: var(--gradient-1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .stat-item:nth-child(2n) .stat-number {
            background: var(--gradient-3);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .stat-item:nth-child(3n) .stat-number {
            background: var(--gradient-4);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .stat-item:nth-child(4n) .stat-number {
            background: var(--gradient-5);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .stat-label {
            font-size: 16px;
            color: #6C757D;
            font-weight: 500;
        }
        
        /* Testimonials Section */
        .testimonials-section {
            padding: 80px 0;
            background-color: white;
        }
        
        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background-color: #F8F9FA;
            border-radius: 15px;
            padding: 30px;
            position: relative;
            border-left: 4px solid var(--accent-color);
        }
        
        .testimonial-card:nth-child(2n) {
            border-left-color: var(--purple-color);
        }
        
        .testimonial-card:nth-child(3n) {
            border-left-color: var(--teal-color);
        }
        
        .testimonial-content {
            font-style: italic;
            margin-bottom: 20px;
            color: #495057;
        }
        
        .testimonial-author {
            display: flex;
            align-items: center;
        }
        
        .author-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 15px;
            object-fit: cover;
        }
        
        .author-info h4 {
            font-size: 16px;
            font-weight: 600;
            margin-bottom: 5px;
        }
        
        .author-info p {
            font-size: 14px;
            color: #6C757D;
        }
        
        /* Mental Health Section */
        .mental-health-section {
            padding: 80px 0;
            background: linear-gradient(135deg, #f5f7fa 0%, #e4eaf5 100%);
        }
        
        .mental-health-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .mental-health-text {
            flex: 1;
        }
        
        .mental-health-image {
            flex: 1;
            text-align: center;
        }
        
        .mental-health-image img {
            max-width: 100%;
            border-radius: 15px;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        /* Login Section */
        .login-section {
            padding: 80px 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: calc(100vh - 200px);
            background: linear-gradient(135deg, #f5f7fa 0%, #e4eaf5 100%);
            position: relative;
            overflow: hidden;
        }
        
        .login-section::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80') center/cover no-repeat;
            opacity: 0.15;
            z-index: 0;
        }
        
        .login-container {
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            padding: 50px;
            width: 100%;
            max-width: 550px;
            position: relative;
            z-index: 1;
            border: 1px solid rgba(255, 255, 255, 0.8);
        }
        
        .login-header {
            text-align: center;
            margin-bottom: 40px;
        }
        
        .login-header h2 {
            font-size: 32px;
            color: var(--primary-color);
            margin-bottom: 15px;
            font-weight: 700;
        }
        
        .login-header p {
            color: var(--dark-color);
            font-size: 16px;
        }
        
        .login-options {
            display: flex;
            flex-direction: column;
            gap: 25px;
            margin-top: 40px;
        }
        
        .login-option {
            padding: 25px;
            border: 2px solid #E9ECEF;
            border-radius: 12px;
            text-align: center;
            cursor: pointer;
            transition: all var(--transition-speed) ease;
            background-color: white;
            position: relative;
            overflow: hidden;
        }
        
        .login-option::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--gradient-1);
            opacity: 0;
            transition: opacity var(--transition-speed) ease;
            z-index: -1;
        }
        
        .login-option:hover {
            border-color: var(--primary-color);
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(14, 64, 138, 0.1);
        }
        
        .login-option:hover::before {
            opacity: 0.05;
        }
        
        .login-option i {
            font-size: 40px;
            color: var(--primary-color);
            margin-bottom: 15px;
            background: rgba(14, 64, 138, 0.1);
            width: 80px;
            height: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            margin: 0 auto 15px;
        }
        
        .login-option h3 {
            font-size: 22px;
            margin-bottom: 10px;
            color: var(--dark-color);
            font-weight: 600;
        }
        
        .login-option p {
            color: #6C757D;
            font-size: 14px;
        }
        
        /* Login Form */
        .login-form {
            display: none;
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            padding: 50px;
            width: 100%;
            max-width: 550px;
            position: relative;
            z-index: 1;
            border: 1px solid rgba(255, 255, 255, 0.8);
        }
        
        .login-form.active {
            display: block;
        }
        
        .login-form-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 30px;
        }
        
        .login-form-header h2 {
            font-size: 28px;
            color: var(--primary-color);
            font-weight: 700;
        }
        
        .back-btn {
            background: rgba(14, 64, 138, 0.1);
            border: none;
            font-size: 20px;
            color: var(--primary-color);
            cursor: pointer;
            transition: all var(--transition-speed) ease;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .back-btn:hover {
            background: var(--primary-color);
            color: white;
        }
        
        .form-group {
            margin-bottom: 25px;
        }
        
        .form-label {
            display: block;
            font-size: 14px;
            font-weight: 600;
            color: var(--dark-color);
            margin-bottom: 10px;
        }
        
        .form-control {
            width: 100%;
            padding: 15px;
            border: 1px solid #CED4DA;
            border-radius: 10px;
            font-size: 14px;
            color: var(--dark-color);
            transition: all var(--transition-speed) ease;
            background-color: #F8F9FA;
        }
        
        .form-control:focus {
            border-color: var(--primary-color);
            outline: none;
            box-shadow: 0 0 0 3px rgba(14, 64, 138, 0.1);
            background-color: white;
        }
        
        .form-text {
            font-size: 12px;
            color: #6C757D;
            margin-top: 5px;
        }
        
        .form-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 30px;
        }
        
        .remember-me {
            display: flex;
            align-items: center;
        }
        
        .remember-me input {
            margin-right: 8px;
            width: 18px;
            height: 18px;
            accent-color: var(--primary-color);
        }
        
        .remember-me label {
            font-size: 14px;
            color: var(--dark-color);
        }
        
        .forgot-password {
            font-size: 14px;
            color: var(--primary-color);
            text-decoration: none;
            transition: color var(--transition-speed) ease;
            font-weight: 500;
        }
        
        .forgot-password:hover {
            color: var(--secondary-color);
            text-decoration: underline;
        }
        
        /* Dashboard Styles */
        .dashboard {
            padding: 40px 0;
            display: none;
            background: linear-gradient(180deg, #F5F7FA 0%, #E4EAF5 100%);
            min-height: 100vh;
        }
        
        .dashboard.active {
            display: block;
        }
        
        .dashboard-header {
            margin-bottom: 40px;
            text-align: center;
        }
        
        .dashboard-header h2 {
            font-size: 36px;
            color: var(--primary-color);
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
            font-weight: 700;
        }
        
        .dashboard-header h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--gradient-1);
            border-radius: 2px;
        }
        
        .dashboard-header p {
            color: var(--dark-color);
            font-size: 16px;
            max-width: 700px;
            margin: 0 auto;
        }
        
        .dashboard-nav {
            display: flex;
            justify-content: center;
            margin-bottom: 40px;
            border-bottom: 1px solid #E9ECEF;
            overflow-x: auto;
            -webkit-overflow-scrolling: touch;
            padding-bottom: 5px;
        }
        
        .dashboard-nav-item {
            padding: 12px 25px;
            cursor: pointer;
            font-weight: 500;
            color: #6C757D;
            border-bottom: 3px solid transparent;
            transition: all var(--transition-speed) ease;
            white-space: nowrap;
            position: relative;
        }
        
        .dashboard-nav-item:hover {
            color: var(--primary-color);
        }
        
        .dashboard-nav-item.active {
            color: var(--primary-color);
            border-bottom-color: var(--primary-color);
            font-weight: 600;
        }
        
        .dashboard-content {
            display: none;
        }
        
        .dashboard-content.active {
            display: block;
        }
        
        /* Card Styles */
        .card {
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.05);
            padding: 30px;
            margin-bottom: 30px;
            transition: all var(--transition-speed) ease;
            border: 1px solid rgba(255, 255, 255, 0.8);
        }
        
        .card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .card-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 25px;
        }
        
        .card-title {
            font-size: 24px;
            font-weight: 600;
            color: var(--dark-color);
            position: relative;
            padding-left: 15px;
        }
        
        .card-title::before {
            content: '';
            position: absolute;
            left: 0;
            top: 50%;
            transform: translateY(-50%);
            width: 5px;
            height: 24px;
            background: var(--gradient-1);
            border-radius: 3px;
        }
        
        .card-body {
            color: #495057;
        }
        
        /* File Upload */
        .file-upload {
            border: 2px dashed #CED4DA;
            border-radius: 12px;
            padding: 50px;
            text-align: center;
            cursor: pointer;
            transition: all var(--transition-speed) ease;
            margin-bottom: 25px;
            background-color: white;
            position: relative;
            overflow: hidden;
        }
        
        .file-upload::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--gradient-1);
            opacity: 0;
            transition: opacity var(--transition-speed) ease;
            z-index: -1;
        }
        
        .file-upload:hover {
            border-color: var(--primary-color);
            background-color: rgba(14, 64, 138, 0.05);
        }
        
        .file-upload:hover::before {
            opacity: 0.03;
        }
        
        .file-upload.drag-over {
            border-color: var(--primary-color);
            background-color: rgba(14, 64, 138, 0.05);
        }
        
        .file-upload i {
            font-size: 60px;
            color: var(--primary-color);
            margin-bottom: 20px;
            background: rgba(14, 64, 138, 0.1);
            width: 100px;
            height: 100px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            margin: 0 auto 20px;
        }
        
        .file-upload h3 {
            font-size: 22px;
            margin-bottom: 15px;
            color: var(--dark-color);
            font-weight: 600;
        }
        
        .file-upload p {
            color: #6C757D;
            font-size: 16px;
            margin-bottom: 20px;
        }
        
        /* Progress Bar */
        .progress-container {
            width: 100%;
            height: 10px;
            background-color: #E9ECEF;
            border-radius: 5px;
            margin: 25px 0;
            overflow: hidden;
        }
        
        .progress-bar {
            height: 100%;
            background: var(--gradient-1);
            border-radius: 5px;
            width: 0%;
            transition: width 0.3s ease;
        }
        
        /* Score Display */
        .score-display {
            display: flex;
            align-items: center;
            margin-top: 30px;
            flex-wrap: wrap;
        }
        
        .score-circle {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 42px;
            font-weight: 700;
            color: white;
            margin-right: 30px;
            position: relative;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
            background: var(--gradient-1);
        }
        
        .score-circle::before {
            content: '';
            position: absolute;
            top: 15px;
            left: 15px;
            right: 15px;
            bottom: 15px;
            border-radius: 50%;
            border: 3px solid rgba(255, 255, 255, 0.3);
        }
        
        .score-excellent {
            background: linear-gradient(135deg, #28A745, #20C997);
        }
        
        .score-good {
            background: linear-gradient(135deg, #17A2B8, #6F42C1);
        }
        
        .score-average {
            background: linear-gradient(135deg, #FFC107, #FD7E14);
        }
        
        .score-poor {
            background: linear-gradient(135deg, #DC3545, #E83E8C);
        }
        
        .score-details {
            flex: 1;
            min-width: 250px;
        }
        
        .score-details h3 {
            font-size: 22px;
            margin-bottom: 15px;
            color: var(--dark-color);
            font-weight: 600;
        }
        
        .score-details p {
            margin-bottom: 10px;
            color: #495057;
            font-size: 16px;
        }
        
        .score-details ul {
            margin-top: 15px;
            padding-left: 20px;
        }
        
        .score-details li {
            margin-bottom: 10px;
            font-size: 15px;
        }
        
        /* Analysis Details */
        .analysis-details {
            margin-top: 30px;
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
            gap: 20px;
        }
        
        .analysis-item {
            background-color: #F8F9FA;
            border-radius: 12px;
            padding: 20px;
            text-align: center;
            transition: all var(--transition-speed) ease;
            border: 1px solid rgba(255, 255, 255, 0.8);
        }
        
        .analysis-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.05);
        }
        
        .analysis-item i {
            font-size: 30px;
            margin-bottom: 15px;
        }
        
        .analysis-item.excellent i {
            color: var(--success-color);
        }
        
        .analysis-item.good i {
            color: var(--info-color);
        }
        
        .analysis-item.average i {
            color: var(--warning-color);
        }
        
        .analysis-item.poor i {
            color: var(--danger-color);
        }
        
        .analysis-label {
            font-size: 16px;
            font-weight: 600;
            color: var(--dark-color);
            margin-bottom: 8px;
        }
        
        .analysis-value {
            font-size: 14px;
            color: #6C757D;
        }
        
        /* Job Postings */
        .job-postings-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .job-card {
            background-color: #F8F9FA;
            border-radius: 12px;
            padding: 20px;
            transition: all var(--transition-speed) ease;
            border: 1px solid rgba(255, 255, 255, 0.8);
        }
        
        .job-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.05);
        }
        
        .job-header {
            display: flex;
            justify-content: space-between;
            align-items: start;
            margin-bottom: 15px;
        }
        
        .job-title {
            font-size: 18px;
            font-weight: 600;
            color: var(--dark-color);
            margin-bottom: 5px;
        }
        
        .job-company {
            font-size: 14px;
            color: #6C757D;
        }
        
        .job-status {
            padding: 4px 8px;
            border-radius: 12px;
            font-size: 12px;
            font-weight: 500;
        }
        
        .job-status.active {
            background-color: rgba(40, 167, 69, 0.1);
            color: var(--success-color);
        }
        
        .job-status.inactive {
            background-color: rgba(220, 53, 69, 0.1);
            color: var(--danger-color);
        }
        
        .job-details {
            margin-bottom: 15px;
        }
        
        .job-detail {
            display: flex;
            align-items: center;
            margin-bottom: 8px;
            font-size: 14px;
            color: #6C757D;
        }
        
        .job-detail i {
            margin-right: 8px;
            color: var(--primary-color);
            width: 16px;
        }
        
        .job-actions {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 15px;
        }
        
        .applicants-count {
            font-size: 14px;
            color: #6C757D;
        }
        
        .applicants-count strong {
            color: var(--primary-color);
        }
        
        /* Candidates List */
        .candidates-list {
            margin-top: 20px;
        }
        
        .candidate-item {
            display: flex;
            align-items: center;
            padding: 15px;
            background-color: #F8F9FA;
            border-radius: 10px;
            margin-bottom: 10px;
            transition: all var(--transition-speed) ease;
        }
        
        .candidate-item:hover {
            background-color: #F1F3F5;
            transform: translateX(5px);
        }
        
        .candidate-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            margin-right: 15px;
            object-fit: cover;
        }
        
        .candidate-info {
            flex: 1;
        }
        
        .candidate-name {
            font-size: 16px;
            font-weight: 600;
            color: var(--dark-color);
            margin-bottom: 5px;
        }
        
        .candidate-email {
            font-size: 14px;
            color: #6C757D;
        }
        
        .candidate-score {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 10px;
            background-color: white;
            border-radius: 8px;
            min-width: 80px;
        }
        
        .score-number {
            font-size: 20px;
            font-weight: 700;
            margin-bottom: 5px;
        }
        
        .score-number.excellent {
            color: var(--success-color);
        }
        
        .score-number.good {
            color: var(--info-color);
        }
        
        .score-number.average {
            color: var(--warning-color);
        }
        
        .score-number.poor {
            color: var(--danger-color);
        }
        
        .score-label {
            font-size: 12px;
            color: #6C757D;
        }
        
        /* Fairness Index */
        .fairness-index-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }
        
        .fairness-metric {
            flex: 1;
            min-width: 200px;
            background-color: #F8F9FA;
            border-radius: 12px;
            padding: 20px;
            text-align: center;
            transition: all var(--transition-speed) ease;
        }
        
        .fairness-metric:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.05);
        }
        
        .metric-icon {
            font-size: 30px;
            margin-bottom: 15px;
        }
        
        .metric-icon.excellent {
            color: var(--success-color);
        }
        
        .metric-icon.good {
            color: var(--info-color);
        }
        
        .metric-icon.average {
            color: var(--warning-color);
        }
        
        .metric-icon.poor {
            color: var(--danger-color);
        }
        
        .metric-value {
            font-size: 32px;
            font-weight: 700;
            margin-bottom: 10px;
        }
        
        .metric-value.excellent {
            color: var(--success-color);
        }
        
        .metric-value.good {
            color: var(--info-color);
        }
        
        .metric-value.average {
            color: var(--warning-color);
        }
        
        .metric-value.poor {
            color: var(--danger-color);
        }
        
        .metric-label {
            font-size: 16px;
            color: var(--dark-color);
            font-weight: 600;
            margin-bottom: 5px;
        }
        
        .metric-description {
            font-size: 14px;
            color: #6C757D;
        }
        
        /* Notification */
        .notification {
            position: fixed;
            top: 25px;
            right: 25px;
            padding: 18px 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            z-index: 1001;
            display: flex;
            align-items: center;
            transform: translateX(150%);
            transition: transform 0.3s ease;
        }
        
        .notification.show {
            transform: translateX(0);
        }
        
        .notification-icon {
            font-size: 22px;
            margin-right: 12px;
        }
        
        .notification-message {
            font-size: 15px;
            color: white;
            font-weight: 500;
        }
        
        .notification-success {
            background: linear-gradient(135deg, #28A745, #20C997);
        }
        
        .notification-error {
            background: linear-gradient(135deg, #DC3545, #E83E8C);
        }
        
        .notification-info {
            background: linear-gradient(135deg, #17A2B8, #6F42C1);
        }
        
        .notification-warning {
            background: linear-gradient(135deg, #FFC107, #FD7E14);
            color: var(--dark-color);
        }
        
        .notification-warning .notification-message {
            color: var(--dark-color);
        }
        
        /* Footer */
        .footer {
            background: var(--gradient-2);
            color: white;
            padding: 50px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            font-size: 20px;
            margin-bottom: 20px;
            font-weight: 600;
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: rgba(255, 255, 255, 0.8);
            text-decoration: none;
            transition: color var(--transition-speed) ease;
        }
        
        .footer-column ul li a:hover {
            color: white;
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 14px;
            color: rgba(255, 255, 255, 0.7);
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 15px;
        }
        
        .social-links a {
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            transition: all var(--transition-speed) ease;
        }
        
        .social-links a:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-3px);
        }
        
        /* Responsive Styles */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
            }
            
            .logo {
                margin-bottom: 15px;
            }
            
            .tagline {
                font-size: 12px;
                text-align: center;
            }
            
            .dashboard-nav {
                overflow-x: auto;
                -webkit-overflow-scrolling: touch;
                padding-bottom: 10px;
            }
            
            .score-display {
                flex-direction: column;
                text-align: center;
            }
            
            .score-circle {
                margin-right: 0;
                margin-bottom: 25px;
            }
            
            .mental-health-content {
                flex-direction: column;
            }
            
            .job-header {
                flex-direction: column;
                align-items: start;
            }
            
            .job-status {
                margin-top: 10px;
            }
            
            .candidate-item {
                flex-direction: column;
                align-items: start;
            }
            
            .candidate-avatar {
                margin-bottom: 10px;
            }
            
            .candidate-score {
                align-self: flex-end;
                margin-top: 10px;
            }
            
            .dashboard-header {
                flex-direction: column;
            }
            
            .dashboard-header-left {
                margin-bottom: 20px;
            }
            
            .user-info {
                margin-right: 0;
                margin-bottom: 15px;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-briefcase"></i>
                    <div>
                        <h1>Smart Hire AI</h1>
                        <div class="tagline">Streamlining hiring with fairness, feedback & well-being</div>
                    </div>
                </div>
                <div class="user-menu">
                    <button class="btn btn-outline" id="loginBtn">Login</button>
                    <button class="btn" id="signupBtn">Sign Up</button>
                </div>
            </div>
        </div>
    </header>
    
    <!-- Hero Section -->
    <section class="hero-section">
        <div class="container">
            <div class="hero-content">
                <h1 class="hero-title">Revolutionizing Recruitment with AI</h1>
                <p class="hero-subtitle">Smart Hire AI transforms the hiring process with intelligent resume scoring, fairness metrics, and personalized career guidance</p>
                <div class="hero-buttons">
                    <button class="btn btn-outline" id="learnMoreBtn">Learn More</button>
                    <button class="btn" id="getStartedBtn">Get Started</button>
                </div>
                <img src="https://images.unsplash.com/photo-1551836022-d5d88e9218df?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80" alt="AI Recruitment" class="hero-image">
            </div>
        </div>
    </section>
    
    <!-- Stats Section -->
    <section class="stats-section">
        <div class="container">
            <div class="stats-grid">
                <div class="stat-item">
                    <div class="stat-number">10K+</div>
                    <div class="stat-label">Resumes Analyzed</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">500+</div>
                    <div class="stat-label">Companies</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">85%</div>
                    <div class="stat-label">Success Rate</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">24/7</div>
                    <div class="stat-label">AI Support</div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Features Section -->
    <section class="features-section" id="featuresSection">
        <div class="container">
            <h2 class="section-title">Powerful Features</h2>
            <p class="section-subtitle">Discover how Smart Hire AI can transform your recruitment process</p>
            
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-file-alt"></i>
                    </div>
                    <h3 class="feature-title">Resume Scoring</h3>
                    <p class="feature-description">AI-powered analysis that evaluates resumes based on skills, experience, and relevance to job requirements</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-balance-scale"></i>
                    </div>
                    <h3 class="feature-title">Fairness Index</h3>
                    <p class="feature-description">Comprehensive metrics to ensure unbiased hiring practices and promote diversity in your workforce</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-user-tie"></i>
                    </div>
                    <h3 class="feature-title">Interview Readiness</h3>
                    <p class="feature-description">Personalized preparation tools and mock interviews to help candidates perform their best</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3 class="feature-title">Skill Gap Analysis</h3>
                    <p class="feature-description">Identify skill gaps and receive personalized recommendations for career development</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-comments"></i>
                    </div>
                    <h3 class="feature-title">AI Assistant</h3>
                    <p class="feature-description">24/7 AI-powered support for candidates and recruiters to answer questions and provide guidance</p>
                </div>
                
                <div class="feature-card">
                    <div class="feature-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3 class="feature-title">Data Security</h3>
                    <p class="feature-description">Enterprise-grade security to protect sensitive candidate and company information</p>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Mental Health Section -->
    <section class="mental-health-section">
        <div class="container">
            <h2 class="section-title">Mental Health Support</h2>
            <p class="section-subtitle">Your well-being matters. Our AI-powered mental health assistant is here to support you throughout your job search journey.</p>
            
            <div class="mental-health-content">
                <div class="mental-health-text">
                    <h3>Job Search Can Be Stressful</h3>
                    <p>We understand that the job search process can take a toll on your mental health. Rejections, uncertainty, and long waiting periods can lead to stress and anxiety.</p>
                    <p>Our AI-powered mental health chatbot is designed to provide emotional support, stress management techniques, and resources to help you maintain your well-being during this challenging time.</p>
                    <div style="margin-top: 30px;">
                        <button class="btn btn-purple">Learn More</button>
                        <button class="btn btn-teal" id="tryChatbotBtn" style="margin-left: 15px;">Try Chatbot</button>
                    </div>
                </div>
                <div class="mental-health-image">
                    <img src="https://images.unsplash.com/photo-1544367567-0f2fcb009e0b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1820&q=80" alt="Mental Health Support">
                </div>
            </div>
        </div>
    </section>
    
    <!-- Testimonials Section -->
    <section class="testimonials-section">
        <div class="container">
            <h2 class="section-title">What Our Users Say</h2>
            <p class="section-subtitle">Hear from candidates and companies who have transformed their hiring experience with Smart Hire AI</p>
            
            <div class="testimonials-grid">
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        "Smart Hire AI helped me land my dream job! The resume scoring feature showed me exactly what recruiters are looking for, and the interview preparation tools were invaluable."
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Sarah Johnson" class="author-avatar">
                        <div class="author-info">
                            <h4>Sarah Johnson</h4>
                            <p>Software Engineer</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        "As a hiring manager, Smart Hire AI has cut our screening time by 60%. The fairness metrics ensure we're building a diverse team while finding the best candidates."
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael Chen" class="author-avatar">
                        <div class="author-info">
                            <h4>Michael Chen</h4>
                            <p>HR Director</p>
                        </div>
                    </div>
                </div>
                
                <div class="testimonial-card">
                    <div class="testimonial-content">
                        "The mental health support feature is a game-changer. Job searching was taking a toll on me, but having someone to talk to made all the difference."
                    </div>
                    <div class="testimonial-author">
                        <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Emma Rodriguez" class="author-avatar">
                        <div class="author-info">
                            <h4>Emma Rodriguez</h4>
                            <p>Marketing Specialist</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Login Section -->
    <section class="login-section" id="loginSection">
        <div class="container">
            <!-- Login Options -->
            <div class="login-container" id="loginOptions">
                <div class="login-header">
                    <h2>Welcome to Smart Hire AI</h2>
                    <p>Please select your login type to continue</p>
                </div>
                <div class="login-options">
                    <div class="login-option" id="candidateLoginOption">
                        <i class="fas fa-user-tie"></i>
                        <h3>Login as Candidate</h3>
                        <p>Access your resume scores, job applications, and career development tools</p>
                    </div>
                    <div class="login-option" id="companyLoginOption">
                        <i class="fas fa-building"></i>
                        <h3>Login as Company</h3>
                        <p>Manage your job postings, view candidates, and track hiring metrics</p>
                    </div>
                </div>
            </div>
            
            <!-- Candidate Login Form -->
            <div class="login-form" id="candidateLoginForm">
                <div class="login-form-header">
                    <h2>Candidate Login</h2>
                    <button class="back-btn" id="backToOptionsFromCandidate">
                        <i class="fas fa-arrow-left"></i>
                    </button>
                </div>
                <form id="candidateLoginFormElement">
                    <div class="form-group">
                        <label for="candidateEmail" class="form-label">Email Address</label>
                        <input type="email" class="form-control" id="candidateEmail" placeholder="Enter your email" required>
                    </div>
                    <div class="form-group">
                        <label for="candidatePassword" class="form-label">Password</label>
                        <input type="password" class="form-control" id="candidatePassword" placeholder="Enter your password" required>
                    </div>
                    <div class="form-footer">
                        <div class="remember-me">
                            <input type="checkbox" id="candidateRemember">
                            <label for="candidateRemember">Remember me</label>
                        </div>
                        <a href="#" class="forgot-password">Forgot password?</a>
                    </div>
                    <button type="submit" class="btn" style="width: 100%; margin-top: 20px;">Login</button>
                    <div class="form-text" style="text-align: center; margin-top: 15px;">
                        Don't have an account? <a href="#" id="candidateSignupLink">Sign up</a>
                    </div>
                </form>
            </div>
            
            <!-- Company Login Form -->
            <div class="login-form" id="companyLoginForm">
                <div class="login-form-header">
                    <h2>Company Login</h2>
                    <button class="back-btn" id="backToOptionsFromCompany">
                        <i class="fas fa-arrow-left"></i>
                    </button>
                </div>
                <form id="companyLoginFormElement">
                    <div class="form-group">
                        <label for="companyEmail" class="form-label">Company Email</label>
                        <input type="email" class="form-control" id="companyEmail" placeholder="Enter your company email" required>
                    </div>
                    <div class="form-group">
                        <label for="companyPassword" class="form-label">Password</label>
                        <input type="password" class="form-control" id="companyPassword" placeholder="Enter your password" required>
                    </div>
                    <div class="form-footer">
                        <div class="remember-me">
                            <input type="checkbox" id="companyRemember">
                            <label for="companyRemember">Remember me</label>
                        </div>
                        <a href="#" class="forgot-password">Forgot password?</a>
                    </div>
                    <button type="submit" class="btn" style="width: 100%; margin-top: 20px;">Login</button>
                    <div class="form-text" style="text-align: center; margin-top: 15px;">
                        Don't have an account? <a href="#" id="companySignupLink">Sign up</a>
                    </div>
                </form>
            </div>
        </div>
    </section>
    
    <!-- Candidate Dashboard -->
    <section class="dashboard" id="candidateDashboard">
        <div class="container">
            <div class="dashboard-header">
                <div class="dashboard-header-left">
                    <h2>Candidate Dashboard</h2>
                    <p>Welcome back! Here's an overview of your job search progress.</p>
                </div>
                <div class="dashboard-header-right">
                    <div class="user-info">
                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="User" class="user-avatar">
                        <div>
                            <div class="user-name">John Doe</div>
                            <div class="user-role">Candidate</div>
                        </div>
                    </div>
                    <button class="btn btn-logout" id="candidateLogoutBtn">
                        <i class="fas fa-sign-out-alt" style="margin-right: 8px;"></i>
                        Logout
                    </button>
                </div>
            </div>
            
            <div class="dashboard-nav">
                <div class="dashboard-nav-item active" data-tab="resume-scoring">Resume Scoring</div>
                <div class="dashboard-nav-item" data-tab="interview-readiness">Interview Readiness</div>
                <div class="dashboard-nav-item" data-tab="job-applications">Job Applications</div>
                <div class="dashboard-nav-item" data-tab="mock-interviews">Mock Interviews</div>
                <div class="dashboard-nav-item" data-tab="skill-tests">Skill Tests</div>
            </div>
            
            <!-- Resume Scoring Tab -->
            <div class="dashboard-content active" id="resume-scoring">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Upload Your Resume</h3>
                    </div>
                    <div class="card-body">
                        <div class="file-upload" id="resumeUpload">
                            <i class="fas fa-cloud-upload-alt"></i>
                            <h3>Drag & Drop Your Resume Here</h3>
                            <p>Supported formats: PDF, DOC, DOCX, TXT (Max size: 5MB)</p>
                            <button class="btn" style="margin-top: 15px;">Browse Files</button>
                        </div>
                        <input type="file" id="resumeFile" accept=".pdf,.doc,.docx,.txt" style="display: none;">
                        <div class="progress-container" id="progressContainer" style="display: none;">
                            <div class="progress-bar" id="progressBar"></div>
                        </div>
                    </div>
                </div>
                
                <div class="card" id="resumeScoreCard" style="display: none;">
                    <div class="card-header">
                        <h3 class="card-title">Your Resume Score</h3>
                    </div>
                    <div class="card-body">
                        <div class="score-display">
                            <div class="score-circle" id="resumeScoreCircle">85</div>
                            <div class="score-details">
                                <h3>Resume Analysis</h3>
                                <p id="resumeAnalysisText">Your resume is well-structured and highlights your key skills effectively.</p>
                                <ul id="resumeAnalysisPoints">
                                    <li>Strengths: Clear formatting, relevant experience</li>
                                    <li>Areas for improvement: Add more quantifiable achievements</li>
                                    <li>Keywords optimization: Good</li>
                                </ul>
                            </div>
                        </div>
                        
                        <div class="analysis-details" id="analysisDetails">
                            <div class="analysis-item" id="educationAnalysis">
                                <i class="fas fa-graduation-cap"></i>
                                <div class="analysis-label">Education</div>
                                <div class="analysis-value">Not found</div>
                            </div>
                            <div class="analysis-item" id="experienceAnalysis">
                                <i class="fas fa-briefcase"></i>
                                <div class="analysis-label">Experience</div>
                                <div class="analysis-value">Not found</div>
                            </div>
                            <div class="analysis-item" id="achievementsAnalysis">
                                <i class="fas fa-trophy"></i>
                                <div class="analysis-label">Achievements</div>
                                <div class="analysis-value">Not found</div>
                            </div>
                            <div class="analysis-item" id="skillsAnalysis">
                                <i class="fas fa-cogs"></i>
                                <div class="analysis-label">Skills</div>
                                <div class="analysis-value">Not found</div>
                            </div>
                            <div class="analysis-item" id="contactAnalysis">
                                <i class="fas fa-address-card"></i>
                                <div class="analysis-label">Contact Info</div>
                                <div class="analysis-value">Not found</div>
                            </div>
                            <div class="analysis-item" id="formatAnalysis">
                                <i class="fas fa-file-alt"></i>
                                <div class="analysis-label">Format</div>
                                <div class="analysis-value">Not analyzed</div>
                            </div>
                        </div>
                        
                        <div style="margin-top: 30px; text-align: center;">
                            <button class="btn" id="downloadReportBtn">
                                <i class="fas fa-download" style="margin-right: 8px;"></i>
                                Download Detailed Report
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Interview Readiness Tab -->
            <div class="dashboard-content" id="interview-readiness">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Your Interview Readiness Score</h3>
                    </div>
                    <div class="card-body">
                        <div class="score-display">
                            <div class="score-circle score-average" id="interviewScoreCircle">72</div>
                            <div class="score-details">
                                <h3>Interview Preparedness</h3>
                                <p>You have a good foundation but could benefit from more practice in specific areas.</p>
                                <ul>
                                    <li>Technical Knowledge: Good</li>
                                    <li>Communication Skills: Average</li>
                                    <li>Problem Solving: Good</li>
                                    <li>Behavioral Responses: Needs Improvement</li>
                                </ul>
                                <button class="btn" style="margin-top: 20px;">
                                    <i class="fas fa-redo" style="margin-right: 8px;"></i>
                                    Take Assessment Again
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Job Applications Tab -->
            <div class="dashboard-content" id="job-applications">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Your Job Applications</h3>
                        <button class="btn btn-success">
                            <i class="fas fa-plus" style="margin-right: 8px;"></i>
                            Find New Jobs
                        </button>
                    </div>
                    <div class="card-body">
                        <div class="job-postings-grid">
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Senior Frontend Developer</div>
                                        <div class="job-company">TechCorp Inc.</div>
                                    </div>
                                    <div class="job-status active">Applied</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>San Francisco, CA</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$120,000 - $150,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Applied 3 days ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Status: <strong>Under Review</strong></div>
                                    <button class="btn btn-sm">View Details</button>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">UX Designer</div>
                                        <div class="job-company">Design Studio</div>
                                    </div>
                                    <div class="job-status active">Applied</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>Remote</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$90,000 - $110,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Applied 1 week ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Status: <strong>Interview Scheduled</strong></div>
                                    <button class="btn btn-sm">View Details</button>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Data Scientist</div>
                                        <div class="job-company">AI Solutions</div>
                                    </div>
                                    <div class="job-status inactive">Rejected</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>New York, NY</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$130,000 - $160,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Applied 2 weeks ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Status: <strong>Not Selected</strong></div>
                                    <button class="btn btn-sm">View Feedback</button>
                                </div>
                            </div>
                        </div>
                        
                        <div style="text-align: center; margin-top: 30px;">
                            <button class="btn btn-outline">View All Applications</button>
                        </div>
                    </div>
                </div>
                
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Application Statistics</h3>
                    </div>
                    <div class="card-body">
                        <div class="fairness-index-container">
                            <div class="fairness-metric">
                                <i class="fas fa-file-import metric-icon good"></i>
                                <div class="metric-value good">24</div>
                                <div class="metric-label">Total Applications</div>
                                <div class="metric-description">Jobs applied to</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-user-check metric-icon excellent"></i>
                                <div class="metric-value excellent">8</div>
                                <div class="metric-label">Interviews</div>
                                <div class="metric-description">Interviews scheduled</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-handshake metric-icon average"></i>
                                <div class="metric-value average">3</div>
                                <div class="metric-label">Offers</div>
                                <div class="metric-description">Job offers received</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-percentage metric-icon good"></i>
                                <div class="metric-value good">33%</div>
                                <div class="metric-label">Response Rate</div>
                                <div class="metric-description">Employer responses</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Mock Interviews Tab -->
            <div class="dashboard-content" id="mock-interviews">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Mock Interview Sessions</h3>
                        <button class="btn btn-success">
                            <i class="fas fa-plus" style="margin-right: 8px;"></i>
                            Schedule New Interview
                        </button>
                    </div>
                    <div class="card-body">
                        <div class="job-postings-grid">
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Technical Interview Practice</div>
                                        <div class="job-company">Software Development</div>
                                    </div>
                                    <div class="job-status active">Completed</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-calendar-alt"></i>
                                        <span>Completed on Jun 15, 2023</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Duration: 45 minutes</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-user"></i>
                                        <span>Interviewer: AI Assistant</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Score: <strong>82/100</strong></div>
                                    <button class="btn btn-sm">View Feedback</button>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Behavioral Interview</div>
                                        <div class="job-company">General Preparation</div>
                                    </div>
                                    <div class="job-status active">Completed</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-calendar-alt"></i>
                                        <span>Completed on Jun 10, 2023</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Duration: 30 minutes</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-user"></i>
                                        <span>Interviewer: AI Assistant</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Score: <strong>75/100</strong></div>
                                    <button class="btn btn-sm">View Feedback</button>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">System Design Interview</div>
                                        <div class="job-company">Senior Position Prep</div>
                                    </div>
                                    <div class="job-status inactive">Scheduled</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-calendar-alt"></i>
                                        <span>Scheduled for Jun 25, 2023</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Duration: 60 minutes</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-user"></i>
                                        <span>Interviewer: AI Assistant</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Status: <strong>Upcoming</strong></div>
                                    <button class="btn btn-sm">Reschedule</button>
                                </div>
                            </div>
                        </div>
                        
                        <div style="text-align: center; margin-top: 30px;">
                            <button class="btn btn-outline">View All Sessions</button>
                        </div>
                    </div>
                </div>
                
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Interview Performance</h3>
                    </div>
                    <div class="card-body">
                        <div class="score-display">
                            <div class="score-circle score-good" id="interviewPerformanceScore">78</div>
                            <div class="score-details">
                                <h3>Overall Interview Performance</h3>
                                <p>Your interview skills have improved over time. Focus on behavioral questions to further enhance your performance.</p>
                                <ul>
                                    <li>Technical Skills: 85/100</li>
                                    <li>Communication: 72/100</li>
                                    <li>Problem Solving: 80/100</li>
                                    <li>Behavioral Responses: 65/100</li>
                                </ul>
                                <button class="btn" style="margin-top: 20px;">
                                    <i class="fas fa-chart-line" style="margin-right: 8px;"></i>
                                    View Detailed Analytics
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Skill Tests Tab -->
            <div class="dashboard-content" id="skill-tests">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Skill Assessment Tests</h3>
                        <button class="btn btn-success">
                            <i class="fas fa-plus" style="margin-right: 8px;"></i>
                            Take New Test
                        </button>
                    </div>
                    <div class="card-body">
                        <div class="job-postings-grid">
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">JavaScript Proficiency</div>
                                        <div class="job-company">Programming Skills</div>
                                    </div>
                                    <div class="job-status active">Completed</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-calendar-alt"></i>
                                        <span>Completed on Jun 12, 2023</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Duration: 45 minutes</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-question-circle"></i>
                                        <span>30 questions</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Score: <strong>88%</strong></div>
                                    <button class="btn btn-sm">View Results</button>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Data Structures & Algorithms</div>
                                        <div class="job-company">Computer Science</div>
                                    </div>
                                    <div class="job-status active">Completed</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-calendar-alt"></i>
                                        <span>Completed on Jun 5, 2023</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Duration: 60 minutes</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-question-circle"></i>
                                        <span>25 questions</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Score: <strong>76%</strong></div>
                                    <button class="btn btn-sm">View Results</button>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">UI/UX Design Principles</div>
                                        <div class="job-company">Design Skills</div>
                                    </div>
                                    <div class="job-status inactive">In Progress</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-calendar-alt"></i>
                                        <span>Started on Jun 20, 2023</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Time remaining: 25 minutes</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-question-circle"></i>
                                        <span>20 questions (15 completed)</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count">Progress: <strong>75%</strong></div>
                                    <button class="btn btn-sm">Continue Test</button>
                                </div>
                            </div>
                        </div>
                        
                        <div style="text-align: center; margin-top: 30px;">
                            <button class="btn btn-outline">View All Tests</button>
                        </div>
                    </div>
                </div>
                
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Skill Analysis</h3>
                    </div>
                    <div class="card-body">
                        <div class="fairness-index-container">
                            <div class="fairness-metric">
                                <i class="fas fa-code metric-icon excellent"></i>
                                <div class="metric-value excellent">88%</div>
                                <div class="metric-label">Programming</div>
                                <div class="metric-description">Average test score</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-project-diagram metric-icon good"></i>
                                <div class="metric-value good">76%</div>
                                <div class="metric-label">Algorithms</div>
                                <div class="metric-description">Problem solving ability</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-paint-brush metric-icon average"></i>
                                <div class="metric-value average">65%</div>
                                <div class="metric-label">Design</div>
                                <div class="metric-description">UI/UX knowledge</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-comments metric-icon good"></i>
                                <div class="metric-value good">82%</div>
                                <div class="metric-label">Communication</div>
                                <div class="metric-description">Soft skills assessment</div>
                            </div>
                        </div>
                        
                        <div style="margin-top: 30px; text-align: center;">
                            <button class="btn btn-purple">
                                <i class="fas fa-download" style="margin-right: 8px;"></i>
                                Download Skill Report
                            </button>
                            <button class="btn btn-teal" style="margin-left: 15px;">
                                <i class="fas fa-lightbulb" style="margin-right: 8px;"></i>
                                Get Learning Recommendations
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Company Dashboard -->
    <section class="dashboard" id="companyDashboard">
        <div class="container">
            <div class="dashboard-header">
                <div class="dashboard-header-left">
                    <h2>Company Dashboard</h2>
                    <p>Welcome back! Here's an overview of your recruitment activities.</p>
                </div>
                <div class="dashboard-header-right">
                    <div class="user-info">
                        <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="User" class="user-avatar">
                        <div>
                            <div class="user-name">Sarah Johnson</div>
                            <div class="user-role">HR Manager</div>
                        </div>
                    </div>
                    <button class="btn btn-logout" id="companyLogoutBtn">
                        <i class="fas fa-sign-out-alt" style="margin-right: 8px;"></i>
                        Logout
                    </button>
                </div>
            </div>
            
            <div class="dashboard-nav">
                <div class="dashboard-nav-item active" data-tab="company-dashboard">Dashboard</div>
                <div class="dashboard-nav-item" data-tab="job-postings">Job Postings</div>
                <div class="dashboard-nav-item" data-tab="fairness-index">Fairness Index</div>
                <div class="dashboard-nav-item" data-tab="analytics">Analytics</div>
            </div>
            
            <!-- Company Dashboard Tab -->
            <div class="dashboard-content active" id="company-dashboard">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Overview</h3>
                    </div>
                    <div class="card-body">
                        <div class="fairness-index-container">
                            <div class="fairness-metric">
                                <i class="fas fa-briefcase metric-icon excellent"></i>
                                <div class="metric-value excellent">12</div>
                                <div class="metric-label">Active Jobs</div>
                                <div class="metric-description">Currently open positions</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-users metric-icon good"></i>
                                <div class="metric-value good">48</div>
                                <div class="metric-label">Total Applicants</div>
                                <div class="metric-description">Candidates applied</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-user-check metric-icon excellent"></i>
                                <div class="metric-value excellent">8</div>
                                <div class="metric-label">Hired</div>
                                <div class="metric-description">Successful placements</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-chart-line metric-icon good"></i>
                                <div class="metric-value good">78%</div>
                                <div class="metric-label">Fairness Score</div>
                                <div class="metric-description">Overall rating</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Recent Activity</h3>
                    </div>
                    <div class="card-body">
                        <div class="job-postings-grid">
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Senior Frontend Developer</div>
                                        <div class="job-company">TechCorp Inc.</div>
                                    </div>
                                    <div class="job-status active">Active</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>San Francisco, CA</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$120,000 - $150,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Posted 3 days ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count"><strong>12</strong> applicants</div>
                                    <button class="btn btn-sm">View Details</button>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">UX Designer</div>
                                        <div class="job-company">Design Studio</div>
                                    </div>
                                    <div class="job-status active">Active</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>Remote</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$90,000 - $110,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Posted 1 week ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count"><strong>8</strong> applicants</div>
                                    <button class="btn btn-sm">View Details</button>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Data Scientist</div>
                                        <div class="job-company">AI Solutions</div>
                                    </div>
                                    <div class="job-status inactive">Closed</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>New York, NY</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$130,000 - $160,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Posted 2 weeks ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count"><strong>15</strong> applicants</div>
                                    <button class="btn btn-sm">View Details</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Job Postings Tab -->
            <div class="dashboard-content" id="job-postings">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Your Job Postings</h3>
                        <button class="btn btn-success">
                            <i class="fas fa-plus" style="margin-right: 8px;"></i>
                            Post New Job
                        </button>
                    </div>
                    <div class="card-body">
                        <div class="job-postings-grid">
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Senior Frontend Developer</div>
                                        <div class="job-company">TechCorp Inc.</div>
                                    </div>
                                    <div class="job-status active">Active</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>San Francisco, CA</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$120,000 - $150,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Posted 3 days ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count"><strong>12</strong> applicants</div>
                                    <button class="btn btn-sm">View Candidates</button>
                                </div>
                                
                                <div class="candidates-list" id="candidates-list-1">
                                    <div class="candidate-item">
                                        <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Sarah Johnson" class="candidate-avatar">
                                        <div class="candidate-info">
                                            <div class="candidate-name">Sarah Johnson</div>
                                            <div class="candidate-email">sarah.johnson@email.com</div>
                                        </div>
                                        <div class="candidate-score">
                                            <div class="score-number excellent">92</div>
                                            <div class="score-label">Score</div>
                                        </div>
                                    </div>
                                    <div class="candidate-item">
                                        <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael Chen" class="candidate-avatar">
                                        <div class="candidate-info">
                                            <div class="candidate-name">Michael Chen</div>
                                            <div class="candidate-email">michael.chen@email.com</div>
                                        </div>
                                        <div class="candidate-score">
                                            <div class="score-number good">85</div>
                                            <div class="score-label">Score</div>
                                        </div>
                                    </div>
                                    <div class="candidate-item">
                                        <img src="https://randomuser.me/api/portraits/women/68.jpg" alt="Emma Rodriguez" class="candidate-avatar">
                                        <div class="candidate-info">
                                            <div class="candidate-name">Emma Rodriguez</div>
                                            <div class="candidate-email">emma.rodriguez@email.com</div>
                                        </div>
                                        <div class="candidate-score">
                                            <div class="score-number excellent">88</div>
                                            <div class="score-label">Score</div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">UX Designer</div>
                                        <div class="job-company">Design Studio</div>
                                    </div>
                                    <div class="job-status active">Active</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>Remote</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$90,000 - $110,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Posted 1 week ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count"><strong>8</strong> applicants</div>
                                    <button class="btn btn-sm">View Candidates</button>
                                </div>
                                
                                <div class="candidates-list" id="candidates-list-2" style="display: none;">
                                    <div class="candidate-item">
                                        <img src="https://randomuser.me/api/portraits/men/75.jpg" alt="David Wilson" class="candidate-avatar">
                                        <div class="candidate-info">
                                            <div class="candidate-name">David Wilson</div>
                                            <div class="candidate-email">david.wilson@email.com</div>
                                        </div>
                                        <div class="candidate-score">
                                            <div class="score-number good">82</div>
                                            <div class="score-label">Score</div>
                                        </div>
                                    </div>
                                    <div class="candidate-item">
                                        <img src="https://randomuser.me/api/portraits/women/28.jpg" alt="Lisa Anderson" class="candidate-avatar">
                                        <div class="candidate-info">
                                            <div class="candidate-name">Lisa Anderson</div>
                                            <div class="candidate-email">lisa.anderson@email.com</div>
                                        </div>
                                        <div class="candidate-score">
                                            <div class="score-number excellent">90</div>
                                            <div class="score-label">Score</div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            
                            <div class="job-card">
                                <div class="job-header">
                                    <div>
                                        <div class="job-title">Data Scientist</div>
                                        <div class="job-company">AI Solutions</div>
                                    </div>
                                    <div class="job-status inactive">Closed</div>
                                </div>
                                <div class="job-details">
                                    <div class="job-detail">
                                        <i class="fas fa-map-marker-alt"></i>
                                        <span>New York, NY</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-dollar-sign"></i>
                                        <span>$130,000 - $160,000</span>
                                    </div>
                                    <div class="job-detail">
                                        <i class="fas fa-clock"></i>
                                        <span>Posted 2 weeks ago</span>
                                    </div>
                                </div>
                                <div class="job-actions">
                                    <div class="applicants-count"><strong>15</strong> applicants</div>
                                    <button class="btn btn-sm">View Candidates</button>
                                </div>
                                
                                <div class="candidates-list" id="candidates-list-3" style="display: none;">
                                    <div class="candidate-item">
                                        <img src="https://randomuser.me/api/portraits/men/67.jpg" alt="James Taylor" class="candidate-avatar">
                                        <div class="candidate-info">
                                            <div class="candidate-name">James Taylor</div>
                                            <div class="candidate-email">james.taylor@email.com</div>
                                        </div>
                                        <div class="candidate-score">
                                            <div class="score-number excellent">94</div>
                                            <div class="score-label">Score</div>
                                        </div>
                                    </div>
                                    <div class="candidate-item">
                                        <img src="https://randomuser.me/api/portraits/women/52.jpg" alt="Jennifer Brown" class="candidate-avatar">
                                        <div class="candidate-info">
                                            <div class="candidate-name">Jennifer Brown</div>
                                            <div class="candidate-email">jennifer.brown@email.com</div>
                                        </div>
                                        <div class="candidate-score">
                                            <div class="score-number good">87</div>
                                            <div class="score-label">Score</div>
                                        </div>
                                    </div>
                                    <div class="candidate-item">
                                        <img src="https://randomuser.me/api/portraits/men/29.jpg" alt="Robert Martinez" class="candidate-avatar">
                                        <div class="candidate-info">
                                            <div class="candidate-name">Robert Martinez</div>
                                            <div class="candidate-email">robert.martinez@email.com</div>
                                        </div>
                                        <div class="candidate-score">
                                            <div class="score-number average">76</div>
                                            <div class="score-label">Score</div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Fairness Index Tab -->
            <div class="dashboard-content" id="fairness-index">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Your Fairness Index Score</h3>
                    </div>
                    <div class="card-body">
                        <div class="score-display">
                            <div class="score-circle score-good">78</div>
                            <div class="score-details">
                                <h3>Fairness Analysis</h3>
                                <p>Your hiring practices show good fairness metrics with room for improvement in certain areas.</p>
                                <ul>
                                    <li>Strengths: Diverse applicant pool, unbiased job descriptions</li>
                                    <li>Areas for improvement: Interview process standardization, reviewer training</li>
                                    <li>Overall rating: Good</li>
                                </ul>
                            </div>
                        </div>
                        
                        <div class="fairness-index-container">
                            <div class="fairness-metric">
                                <i class="fas fa-users metric-icon excellent"></i>
                                <div class="metric-value excellent">92%</div>
                                <div class="metric-label">Diversity Score</div>
                                <div class="metric-description">Applicant diversity representation</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-file-alt metric-icon good"></i>
                                <div class="metric-value good">85%</div>
                                <div class="metric-label">Job Description Bias</div>
                                <div class="metric-description">Neutral language in postings</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-user-tie metric-icon average"></i>
                                <div class="metric-value average">72%</div>
                                <div class="metric-label">Interview Process</div>
                                <div class="metric-description">Standardized evaluation</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-chart-pie metric-icon good"></i>
                                <div class="metric-value good">80%</div>
                                <div class="metric-label">Selection Consistency</div>
                                <div class="metric-description">Hiring decision patterns</div>
                            </div>
                        </div>
                        
                        <div style="margin-top: 30px; text-align: center;">
                            <button class="btn btn-purple">
                                <i class="fas fa-download" style="margin-right: 8px;"></i>
                                Download Fairness Report
                            </button>
                            <button class="btn btn-teal" style="margin-left: 15px;">
                                <i class="fas fa-lightbulb" style="margin-right: 8px;"></i>
                                Get Improvement Tips
                            </button>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Analytics Tab -->
            <div class="dashboard-content" id="analytics">
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Hiring Analytics</h3>
                    </div>
                    <div class="card-body">
                        <div class="fairness-index-container">
                            <div class="fairness-metric">
                                <i class="fas fa-eye metric-icon excellent"></i>
                                <div class="metric-value excellent">1,245</div>
                                <div class="metric-label">Total Views</div>
                                <div class="metric-description">Job post views this month</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-file-import metric-icon good"></i>
                                <div class="metric-value good">342</div>
                                <div class="metric-label">Applications</div>
                                <div class="metric-description">Total applications received</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-user-check metric-icon excellent"></i>
                                <div class="metric-value excellent">28</div>
                                <div class="metric-label">Interviews</div>
                                <div class="metric-description">Candidates interviewed</div>
                            </div>
                            <div class="fairness-metric">
                                <i class="fas fa-handshake metric-icon good"></i>
                                <div class="metric-value good">12</div>
                                <div class="metric-label">Hires</div>
                                <div class="metric-description">Successful placements</div>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="card">
                    <div class="card-header">
                        <h3 class="card-title">Application Funnel</h3>
                    </div>
                    <div class="card-body">
                        <div style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 20px;">
                            <div style="text-align: center;">
                                <div style="font-size: 24px; font-weight: 700; color: var(--primary-color);">1,245</div>
                                <div style="font-size: 14px; color: #6C757D;">Views</div>
                            </div>
                            <i class="fas fa-arrow-right" style="color: #6C757D;"></i>
                            <div style="text-align: center;">
                                <div style="font-size: 24px; font-weight: 700; color: var(--primary-color);">342</div>
                                <div style="font-size: 14px; color: #6C757D;">Applications</div>
                            </div>
                            <i class="fas fa-arrow-right" style="color: #6C757D;"></i>
                            <div style="text-align: center;">
                                <div style="font-size: 24px; font-weight: 700; color: var(--primary-color);">28</div>
                                <div style="font-size: 14px; color: #6C757D;">Interviews</div>
                            </div>
                            <i class="fas fa-arrow-right" style="color: #6C757D;"></i>
                            <div style="text-align: center;">
                                <div style="font-size: 24px; font-weight: 700; color: var(--primary-color);">12</div>
                                <div style="font-size: 14px; color: #6C757D;">Hires</div>
                            </div>
                        </div>
                        
                        <div style="background-color: #F8F9FA; border-radius: 10px; padding: 20px;">
                            <div style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                                <span>View to Application Rate</span>
                                <span style="font-weight: 600;">27.5%</span>
                            </div>
                            <div style="display: flex; justify-content: space-between; margin-bottom: 10px;">
                                <span>Application to Interview Rate</span>
                                <span style="font-weight: 600;">8.2%</span>
                            </div>
                            <div style="display: flex; justify-content: space-between;">
                                <span>Interview to Hire Rate</span>
                                <span style="font-weight: 600;">42.9%</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>Smart Hire AI</h3>
                    <p>Revolutionizing recruitment with AI-powered solutions for fair and efficient hiring.</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                
                <div class="footer-column">
                    <h3>For Candidates</h3>
                    <ul>
                        <li><a href="#">Resume Scoring</a></li>
                        <li><a href="#">Interview Preparation</a></li>
                        <li><a href="#">Skill Assessment</a></li>
                        <li><a href="#">Career Guidance</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>For Companies</h3>
                    <ul>
                        <li><a href="#">Job Posting</a></li>
                        <li><a href="#">Candidate Screening</a></li>
                        <li><a href="#">Fairness Metrics</a></li>
                        <li><a href="#">Analytics Dashboard</a></li>
                    </ul>
                </div>
                
                <div class="footer-column">
                    <h3>Resources</h3>
                    <ul>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Help Center</a></li>
                        <li><a href="#">Privacy Policy</a></li>
                        <li><a href="#">Terms of Service</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2023 Smart Hire AI. All rights reserved.</p>
            </div>
        </div>
    </footer>
    
    <!-- Notification -->
    <div class="notification" id="notification">
        <i class="notification-icon fas fa-check-circle"></i>
        <div class="notification-message">Action completed successfully!</div>
    </div>
    
    <script>
        // DOM Elements
        const loginSection = document.getElementById('loginSection');
        const candidateDashboard = document.getElementById('candidateDashboard');
        const companyDashboard = document.getElementById('companyDashboard');
        const featuresSection = document.getElementById('featuresSection');
        
        // Hero buttons
        const learnMoreBtn = document.getElementById('learnMoreBtn');
        const getStartedBtn = document.getElementById('getStartedBtn');
        
        // Login options
        const loginOptions = document.getElementById('loginOptions');
        const candidateLoginOption = document.getElementById('candidateLoginOption');
        const companyLoginOption = document.getElementById('companyLoginOption');
        
        // Login forms
        const candidateLoginForm = document.getElementById('candidateLoginForm');
        const companyLoginForm = document.getElementById('companyLoginForm');
        const candidateLoginFormElement = document.getElementById('candidateLoginFormElement');
        const companyLoginFormElement = document.getElementById('companyLoginFormElement');
        
        // Back buttons
        const backToOptionsFromCandidate = document.getElementById('backToOptionsFromCandidate');
        const backToOptionsFromCompany = document.getElementById('backToOptionsFromCompany');
        
        // Form inputs
        const candidateEmail = document.getElementById('candidateEmail');
        const candidatePassword = document.getElementById('candidatePassword');
        const companyEmail = document.getElementById('companyEmail');
        const companyPassword = document.getElementById('companyPassword');
        
        // Resume upload
        const resumeUpload = document.getElementById('resumeUpload');
        const resumeFile = document.getElementById('resumeFile');
        const resumeScoreCard = document.getElementById('resumeScoreCard');
        const progressContainer = document.getElementById('progressContainer');
        const progressBar = document.getElementById('progressBar');
        
        // Analysis details elements
        const educationAnalysis = document.getElementById('educationAnalysis');
        const experienceAnalysis = document.getElementById('experienceAnalysis');
        const achievementsAnalysis = document.getElementById('achievementsAnalysis');
        const skillsAnalysis = document.getElementById('skillsAnalysis');
        const contactAnalysis = document.getElementById('contactAnalysis');
        const formatAnalysis = document.getElementById('formatAnalysis');
        
        // Dashboard navigation
        const dashboardNavItems = document.querySelectorAll('.dashboard-nav-item');
        const dashboardContents = document.querySelectorAll('.dashboard-content');
        
        // Modals and notifications
        const notification = document.getElementById('notification');
        const downloadReportBtn = document.getElementById('downloadReportBtn');
        
        // Logout buttons
        const candidateLogoutBtn = document.getElementById('candidateLogoutBtn');
        const companyLogoutBtn = document.getElementById('companyLogoutBtn');
        
        // Store analysis results globally
        let currentAnalysisResults = null;
        let currentUserType = null;
        
        // Hero button functionality
        learnMoreBtn.addEventListener('click', () => {
            featuresSection.scrollIntoView({ behavior: 'smooth' });
        });
        
        getStartedBtn.addEventListener('click', () => {
            // Hide dashboards if they're visible
            candidateDashboard.style.display = 'none';
            companyDashboard.style.display = 'none';
            
            // Show login section
            loginSection.style.display = 'flex';
            loginSection.scrollIntoView({ behavior: 'smooth' });
            
            // Reset login forms
            loginOptions.style.display = 'block';
            candidateLoginForm.style.display = 'none';
            companyLoginForm.style.display = 'none';
            candidateLoginFormElement.reset();
            companyLoginFormElement.reset();
            
            // Reset dashboard navigation
            dashboardNavItems.forEach(item => {
                item.classList.remove('active');
            });
            dashboardContents.forEach(content => {
                content.classList.remove('active');
            });
            
            // Set first tab as active
            if (dashboardNavItems.length > 0) {
                dashboardNavItems[0].classList.add('active');
            }
            if (dashboardContents.length > 0) {
                dashboardContents[0].classList.add('active');
            }
            
            showNotification('Please login to continue', 'info');
        });
        
        // Login option handlers
        candidateLoginOption.addEventListener('click', () => {
            loginOptions.style.display = 'none';
            candidateLoginForm.style.display = 'block';
        });
        
        companyLoginOption.addEventListener('click', () => {
            loginOptions.style.display = 'none';
            companyLoginForm.style.display = 'block';
        });
        
        // Back to options handlers
        backToOptionsFromCandidate.addEventListener('click', () => {
            candidateLoginForm.style.display = 'none';
            loginOptions.style.display = 'block';
            candidateLoginFormElement.reset();
        });
        
        backToOptionsFromCompany.addEventListener('click', () => {
            companyLoginForm.style.display = 'none';
            loginOptions.style.display = 'block';
            companyLoginFormElement.reset();
        });
        
        // Form submission handlers
        candidateLoginFormElement.addEventListener('submit', (e) => {
            e.preventDefault();
            
            const email = candidateEmail.value;
            const password = candidatePassword.value;
            
            // Simple validation
            if (!email || !password) {
                showNotification('Please fill in all fields', 'error');
                return;
            }
            
            // Basic email validation
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailRegex.test(email)) {
                showNotification('Please enter a valid email address', 'error');
                return;
            }
            
            // Simulate login process
            showNotification('Logging in...', 'info');
            
            setTimeout(() => {
                loginSection.style.display = 'none';
                candidateDashboard.style.display = 'block';
                currentUserType = 'candidate';
                showNotification('Logged in successfully as Candidate', 'success');
            }, 1500);
        });
        
        companyLoginFormElement.addEventListener('submit', (e) => {
            e.preventDefault();
            
            const email = companyEmail.value;
            const password = companyPassword.value;
            
            // Simple validation
            if (!email || !password) {
                showNotification('Please fill in all fields', 'error');
                return;
            }
            
            // Basic email validation
            const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailRegex.test(email)) {
                showNotification('Please enter a valid email address', 'error');
                return;
            }
            
            // Simulate login process
            showNotification('Logging in...', 'info');
            
            setTimeout(() => {
                loginSection.style.display = 'none';
                companyDashboard.style.display = 'block';
                currentUserType = 'company';
                showNotification('Logged in successfully as Company', 'success');
            }, 1500);
        });
        
        // Logout button handlers
        candidateLogoutBtn.addEventListener('click', () => {
            // Hide dashboard
            candidateDashboard.style.display = 'none';
            
            // Show login section
            loginSection.style.display = 'flex';
            loginSection.scrollIntoView({ behavior: 'smooth' });
            
            // Reset login forms
            loginOptions.style.display = 'block';
            candidateLoginForm.style.display = 'none';
            companyLoginForm.style.display = 'none';
            candidateLoginFormElement.reset();
            companyLoginFormElement.reset();
            
            // Reset dashboard navigation
            dashboardNavItems.forEach(item => {
                item.classList.remove('active');
            });
            dashboardContents.forEach(content => {
                content.classList.remove('active');
            });
            
            // Set first tab as active
            if (dashboardNavItems.length > 0) {
                dashboardNavItems[0].classList.add('active');
            }
            if (dashboardContents.length > 0) {
                dashboardContents[0].classList.add('active');
            }
            
            currentUserType = null;
            showNotification('Logged out successfully', 'success');
        });
        
        companyLogoutBtn.addEventListener('click', () => {
            // Hide dashboard
            companyDashboard.style.display = 'none';
            
            // Show login section
            loginSection.style.display = 'flex';
            loginSection.scrollIntoView({ behavior: 'smooth' });
            
            // Reset login forms
            loginOptions.style.display = 'block';
            candidateLoginForm.style.display = 'none';
            companyLoginForm.style.display = 'none';
            candidateLoginFormElement.reset();
            companyLoginFormElement.reset();
            
            // Reset dashboard navigation
            dashboardNavItems.forEach(item => {
                item.classList.remove('active');
            });
            dashboardContents.forEach(content => {
                content.classList.remove('active');
            });
            
            // Set first tab as active
            if (dashboardNavItems.length > 0) {
                dashboardNavItems[0].classList.add('active');
            }
            if (dashboardContents.length > 0) {
                dashboardContents[0].classList.add('active');
            }
            
            currentUserType = null;
            showNotification('Logged out successfully', 'success');
        });
        
        // Dashboard navigation
        dashboardNavItems.forEach(item => {
            item.addEventListener('click', () => {
                const tabId = item.getAttribute('data-tab');
                
                // Update active nav item
                dashboardNavItems.forEach(navItem => {
                    navItem.classList.remove('active');
                });
                item.classList.add('active');
                
                // Update active content
                dashboardContents.forEach(content => {
                    content.classList.remove('active');
                });
                document.getElementById(tabId).classList.add('active');
            });
        });
        
        // Drag and drop functionality
        ['dragenter', 'dragover', 'dragleave', 'drop'].forEach(eventName => {
            resumeUpload.addEventListener(eventName, preventDefaults, false);
        });
        
        function preventDefaults(e) {
            e.preventDefault();
            e.stopPropagation();
        }
        
        ['dragenter', 'dragover'].forEach(eventName => {
            resumeUpload.addEventListener(eventName, highlight, false);
        });
        
        ['dragleave', 'drop'].forEach(eventName => {
            resumeUpload.addEventListener(eventName, unhighlight, false);
        });
        
        function highlight() {
            resumeUpload.classList.add('drag-over');
        }
        
        function unhighlight() {
            resumeUpload.classList.remove('drag-over');
        }
        
        resumeUpload.addEventListener('drop', handleDrop, false);
        
        function handleDrop(e) {
            const dt = e.dataTransfer;
            const files = dt.files;
            
            if (files.length) {
                resumeFile.files = files;
                const event = new Event('change', { bubbles: true });
                resumeFile.dispatchEvent(event);
            }
        }
        
        // Resume upload
        resumeUpload.addEventListener('click', () => {
            resumeFile.click();
        });
        
        resumeFile.addEventListener('change', (e) => {
            const file = e.target.files[0];
            if (file) {
                const validTypes = ['application/pdf', 'application/msword', 'application/vnd.openxmlformats-officedocument.wordprocessingml.document', 'text/plain'];
                
                if (validTypes.includes(file.type)) {
                    // Show progress bar
                    progressContainer.style.display = 'block';
                    progressBar.style.width = '0%';
                    
                    // Show loading state
                    resumeUpload.innerHTML = `
                        <i class="fas fa-spinner fa-spin"></i>
                        <h3>Uploading and analyzing your resume...</h3>
                        <p>This may take a few moments</p>
                    `;
                    
                    // Simulate progress
                    let progress = 0;
                    const progressInterval = setInterval(() => {
                        progress += 10;
                        progressBar.style.width = `${progress}%`;
                        
                        if (progress >= 100) {
                            clearInterval(progressInterval);
                            
                            // Simulate analysis after upload completes
                            setTimeout(() => {
                                analyzeResume(file);
                            }, 500);
                        }
                    }, 200);
                } else {
                    showNotification('Please upload a valid resume file (PDF, DOC, DOCX, TXT)', 'error');
                }
            }
        });
        
        // Function to analyze resume
        function analyzeResume(file) {
            // For text files, we can read the content directly
            if (file.type === 'text/plain') {
                const reader = new FileReader();
                reader.onload = function(e) {
                    const content = e.target.result;
                    performResumeAnalysis(content, file.name, file);
                };
                reader.readAsText(file);
            } else {
                // For PDF/DOC files, we'll simulate analysis based on filename and content type
                simulateResumeAnalysis(file);
            }
        }
        
        // Improved performResumeAnalysis function
        function performResumeAnalysis(content, fileName, file) {
            // Convert to lowercase for case-insensitive matching
            const contentLower = content.toLowerCase();
            const fileNameLower = fileName.toLowerCase();
            
            // Enhanced non-resume indicators
            const nonResumeKeywords = [
                'poem', 'poetry', 'verse', 'story', 'novel', 'book', 'article', 'essay', 
                'report', 'thesis', 'dissertation', 'manual', 'guide', 'tutorial', 
                'presentation', 'slides', 'brochure', 'flyer', 'newsletter', 'magazine',
                'newspaper', 'journal', 'research', 'paper', 'publication', 'catalog',
                'invoice', 'receipt', 'contract', 'agreement', 'form', 'application',
                'certificate', 'diploma', 'transcript', 'schedule', 'calendar', 'menu'
            ];
            
            // Check for clear non-resume indicators in filename or content
            const isNonResume = nonResumeKeywords.some(keyword => 
                fileNameLower.includes(keyword) || contentLower.includes(keyword)
            );
            
            // Check for resume-related keywords
            const resumeKeywords = ['resume', 'cv', 'curriculum', 'vitae', 'bio', 'biography'];
            const hasResumeKeyword = resumeKeywords.some(keyword => 
                fileNameLower.includes(keyword) || contentLower.includes(keyword)
            );
            
            // If it's clearly not a resume, give it a zero score
            if (isNonResume && !hasResumeKeyword) {
                currentAnalysisResults = {
                    score: 0,
                    hasEducation: false,
                    hasExperience: false,
                    hasAchievements: false,
                    hasSkills: false,
                    hasContact: false,
                    isPoem: false,
                    isNonResume: true,
                    analysisText: 'This document does not appear to be a resume. Please upload a resume document.',
                    analysisPoints: `
                        <li>This document is not a resume</li>
                        <li>Please upload a proper resume file</li>
                        <li>Include education, experience, and skills sections</li>
                    `,
                    fileName: file.name,
                    fileSize: file.size,
                    fileType: file.type
                };
                updateResumeAnalysisUI();
                return;
            }
            
            // Improved pattern matching for resume sections
            const hasEducation = detectSection(contentLower, [
                'education', 'educational background', 'academic background', 'academic qualifications',
                'qualification', 'qualifications', 'degree', 'degrees', 'university', 'college',
                'institution', 'b.tech', 'm.tech', 'bachelor', 'master', 'phd', 'gpa'
            ]);
            
            const hasExperience = detectSection(contentLower, [
                'experience', 'work experience', 'professional experience', 'employment history',
                'work history', 'career', 'professional background', 'job experience',
                'internship', 'internships', 'employment', 'work', 'professional'
            ]);
            
            const hasAchievements = detectSection(contentLower, [
                'achievements', 'accomplishments', 'awards', 'honors', 'recognition',
                'publications', 'projects', 'certifications', 'achievements', 'accomplishment'
            ]);
            
            const hasSkills = detectSection(contentLower, [
                'skills', 'technical skills', 'professional skills', 'core competencies',
                'expertise', 'competencies', 'abilities', 'proficiencies', 'skill set'
            ]);
            
            const hasContact = detectSection(contentLower, [
                'contact', 'contact information', 'contact details', 'personal details',
                'get in touch', 'reach me', 'email', 'phone', 'address', 'linkedin'
            ]);
            
            // Define poem indicators
            const poemKeywords = ['poem', 'poetry', 'verse', 'stanza', 'rhyme', 'meter', 'sonnet', 'haiku', 'lyric', 'ode'];
            
            // Check if it's likely a poem
            const hasPoemKeywords = poemKeywords.some(keyword => contentLower.includes(keyword) || fileNameLower.includes(keyword));
            
            // Check for resume-specific patterns
            const hasResumePatterns = checkResumePatterns(contentLower);
            
            // Determine if it's a poem or resume
            const isPoem = hasPoemKeywords && !hasExperience && !hasSkills && !hasResumePatterns;
            
            // If it's a poem, give it a zero score
            if (isPoem) {
                currentAnalysisResults = {
                    score: 0,
                    hasEducation: false,
                    hasExperience: false,
                    hasAchievements: false,
                    hasSkills: false,
                    hasContact: false,
                    isPoem: true,
                    isNonResume: true,
                    analysisText: 'This document appears to be a poem, not a resume. Please upload a proper resume document.',
                    analysisPoints: `
                        <li>This is not a resume document</li>
                        <li>Please upload a resume with proper sections</li>
                        <li>Include education, experience, and skills sections</li>
                    `,
                    fileName: file.name,
                    fileSize: file.size,
                    fileType: file.type
                };
                updateResumeAnalysisUI();
                return;
            }
            
            // If no resume sections are detected, give it a zero score
            if (!hasEducation && !hasExperience && !hasSkills && !hasContact) {
                currentAnalysisResults = {
                    score: 0,
                    hasEducation: false,
                    hasExperience: false,
                    hasAchievements: false,
                    hasSkills: false,
                    hasContact: false,
                    isPoem: false,
                    isNonResume: true,
                    analysisText: 'This document does not appear to be a resume. Please upload a resume document.',
                    analysisPoints: `
                        <li>No resume sections detected</li>
                        <li>Please upload a proper resume file</li>
                        <li>Include education, experience, and skills sections</li>
                    `,
                    fileName: file.name,
                    fileSize: file.size,
                    fileType: file.type
                };
                updateResumeAnalysisUI();
                return;
            }
            
            // Calculate score based on sections found and quality indicators
            let score = 0;
            let analysisText = '';
            let analysisPoints = '';
            
            // Base score for having resume sections
            if (hasEducation) score += 20;
            if (hasExperience) score += 25;
            if (hasAchievements) score += 20;
            if (hasSkills) score += 20;
            if (hasContact) score += 10;
            
            // Additional quality checks
            if (hasResumePatterns) score += 5; // Has resume-like structure
            
            // Check for professional action verbs
            const actionVerbs = ['developed', 'managed', 'created', 'implemented', 'led', 'designed', 
                                'analyzed', 'improved', 'increased', 'decreased', 'optimized', 
                                'built', 'launched', 'coordinated', 'achieved', 'established'];
            const actionVerbCount = actionVerbs.filter(verb => contentLower.includes(verb)).length;
            if (actionVerbCount > 3) score += 5;
            if (actionVerbCount > 6) score += 5; // Extra points for strong action verbs
            
            // Check for quantifiable results
            const quantifiablePatterns = [
                /\d+%/, /\d+\s*(percent|per cent)/, /\$\d+/, /\d+\s*(dollars|USD)/,
                /\d+\s*(years|months|weeks|days)/, /\d+\s*(people|users|customers)/
            ];
            const hasQuantifiableResults = quantifiablePatterns.some(pattern => pattern.test(contentLower));
            if (hasQuantifiableResults) score += 5;
            
            // Check for length (good resumes are typically 300-1000 words)
            const wordCount = content.split(/\s+/).length;
            if (wordCount >= 300 && wordCount <= 1000) score += 5;
            else if (wordCount > 1000) score += 2; // Too long but still has content
            
            // Check for keywords related to specific industries (add variety to scores)
            const techKeywords = ['javascript', 'python', 'java', 'react', 'angular', 'node.js', 'html', 'css', 'sql', 'mongodb'];
            const businessKeywords = ['management', 'leadership', 'strategy', 'marketing', 'sales', 'revenue', 'growth'];
            const designKeywords = ['photoshop', 'illustrator', 'figma', 'sketch', 'ui', 'ux', 'design'];
            
            const hasTechKeywords = techKeywords.some(keyword => contentLower.includes(keyword));
            const hasBusinessKeywords = businessKeywords.some(keyword => contentLower.includes(keyword));
            const hasDesignKeywords = designKeywords.some(keyword => contentLower.includes(keyword));
            
            // Add points for industry-specific keywords
            if (hasTechKeywords) score += 3;
            if (hasBusinessKeywords) score += 3;
            if (hasDesignKeywords) score += 3;
            
            // Check for education quality indicators
            const educationQuality = checkEducationQuality(contentLower);
            score += educationQuality;
            
            // Check for experience quality indicators
            const experienceQuality = checkExperienceQuality(contentLower);
            score += experienceQuality;
            
            // Add some randomness to make scores more varied
            score += Math.floor(Math.random() * 10) - 5; // Random between -5 and +5
            
            // Ensure minimum score for non-poem files with some content
            if (score < 50 && (hasEducation || hasExperience || hasSkills)) {
                score = 50 + Math.floor(Math.random() * 15);
            }
            
            // Cap score at 100
            score = Math.max(0, Math.min(score, 100));
            
            // Set analysis text based on score
            if (score >= 90) {
                analysisText = 'Excellent! Your resume is well-structured and effectively showcases your skills and experience.';
                analysisPoints = `
                    <li>Strengths: Clear formatting, strong achievements, relevant keywords, quantifiable results</li>
                    <li>Areas for improvement: Consider adding more industry-specific certifications</li>
                    <li>Keywords optimization: Excellent</li>
                `;
            } else if (score >= 80) {
                analysisText = 'Your resume is well-structured and highlights your key skills effectively.';
                analysisPoints = `
                    <li>Strengths: Clear formatting, relevant experience, good use of action verbs</li>
                    <li>Areas for improvement: Add more quantifiable achievements</li>
                    <li>Keywords optimization: Good</li>
                `;
            } else if (score >= 70) {
                analysisText = 'Your resume has a good foundation but could benefit from some improvements.';
                analysisPoints = `
                    <li>Strengths: Relevant experience listed, basic structure present</li>
                    <li>Areas for improvement: Better formatting, more achievements, quantifiable results</li>
                    <li>Keywords optimization: Average</li>
                `;
            } else if (score >= 50) {
                analysisText = 'Your resume needs significant improvements to effectively showcase your skills.';
                analysisPoints = `
                    <li>Strengths: Basic information included</li>
                    <li>Areas for improvement: Complete restructuring, add achievements, use action verbs</li>
                    <li>Keywords optimization: Poor</li>
                `;
            } else {
                analysisText = 'This document does not appear to be a properly formatted resume.';
                analysisPoints = `
                    <li>Missing essential resume sections</li>
                    <li>Consider restructuring with standard resume format</li>
                    <li>Include education, experience, and skills sections</li>
                `;
            }
            
            // Store analysis results globally
            currentAnalysisResults = {
                score,
                hasEducation,
                hasExperience,
                hasAchievements,
                hasSkills,
                hasContact,
                isPoem: false,
                isNonResume: false,
                analysisText,
                analysisPoints,
                fileName: file.name,
                fileSize: file.size,
                fileType: file.type
            };
            
            // Update UI with analysis results
            updateResumeAnalysisUI();
        }
        
        // Function to check education quality
        function checkEducationQuality(content) {
            let score = 0;
            
            // Check for degree mentions
            if (content.includes('bachelor') || content.includes('master') || content.includes('phd')) {
                score += 2;
            }
            
            // Check for GPA
            if (content.includes('gpa')) {
                score += 1;
            }
            
            // Check for university names
            if (content.includes('university') || content.includes('college')) {
                score += 1;
            }
            
            // Check for graduation years
            if (/\b(19|20)\d{2}\b/.test(content)) {
                score += 1;
            }
            
            return score;
        }
        
        // Function to check experience quality
        function checkExperienceQuality(content) {
            let score = 0;
            
            // Check for company names
            if (content.includes('inc') || content.includes('ltd') || content.includes('llc')) {
                score += 1;
            }
            
            // Check for job titles
            const jobTitles = ['engineer', 'developer', 'manager', 'director', 'analyst', 'specialist', 'consultant'];
            if (jobTitles.some(title => content.includes(title))) {
                score += 2;
            }
            
            // Check for duration of experience
            if (content.includes('year') || content.includes('years')) {
                score += 1;
            }
            
            return score;
        }
        
        // Improved simulateResumeAnalysis function
        function simulateResumeAnalysis(file) {
            const fileName = file.name.toLowerCase();
            
            // Enhanced non-resume indicators
            const nonResumeKeywords = [
                'poem', 'poetry', 'verse', 'story', 'novel', 'book', 'article', 'essay', 
                'report', 'thesis', 'dissertation', 'manual', 'guide', 'tutorial', 
                'presentation', 'slides', 'brochure', 'flyer', 'newsletter', 'magazine',
                'newspaper', 'journal', 'research', 'paper', 'publication', 'catalog',
                'invoice', 'receipt', 'contract', 'agreement', 'form', 'application',
                'certificate', 'diploma', 'transcript', 'schedule', 'calendar', 'menu'
            ];
            
            // Check for clear non-resume indicators in filename
            const isNonResume = nonResumeKeywords.some(keyword => fileName.includes(keyword));
            
            // Check for resume-related keywords
            const resumeKeywords = ['resume', 'cv', 'curriculum', 'vitae', 'bio', 'biography'];
            const hasResumeKeyword = resumeKeywords.some(keyword => fileName.includes(keyword));
            
            // If it's clearly not a resume, give it a zero score
            if (isNonResume && !hasResumeKeyword) {
                currentAnalysisResults = {
                    score: 0,
                    hasEducation: false,
                    hasExperience: false,
                    hasAchievements: false,
                    hasSkills: false,
                    hasContact: false,
                    isPoem: false,
                    isNonResume: true,
                    analysisText: 'This document does not appear to be a resume. Please upload a resume document.',
                    analysisPoints: `
                        <li>This document is not a resume</li>
                        <li>Please upload a proper resume file</li>
                        <li>Include education, experience, and skills sections</li>
                    `,
                    fileName: file.name,
                    fileSize: file.size,
                    fileType: file.type
                };
                updateResumeAnalysisUI();
                return;
            }
            
            // If no clear resume indicators, give it a zero score
            if (!hasResumeKeyword) {
                currentAnalysisResults = {
                    score: 0,
                    hasEducation: false,
                    hasExperience: false,
                    hasAchievements: false,
                    hasSkills: false,
                    hasContact: false,
                    isPoem: false,
                    isNonResume: true,
                    analysisText: 'This document does not appear to be a resume. Please upload a resume document.',
                    analysisPoints: `
                        <li>This document does not contain resume keywords</li>
                        <li>Please upload a proper resume file</li>
                        <li>Include education, experience, and skills sections</li>
                    `,
                    fileName: file.name,
                    fileSize: file.size,
                    fileType: file.type
                };
                updateResumeAnalysisUI();
                return;
            }
            
            // Generate a more realistic score based on file characteristics
            let score = 40; // Base score for files with resume keywords
            
            // Check for name indicators (resumes often include the person's name)
            if (fileName.includes('_') || fileName.includes('-')) {
                score += 5;
            }
            
            // Check for year indicators (resumes often include graduation years)
            if (/\b(19|20)\d{2}\b/.test(fileName)) {
                score += 5;
            }
            
            // Check for common resume file extensions
            if (fileName.endsWith('.pdf') || fileName.endsWith('.doc') || fileName.endsWith('.docx')) {
                score += 5;
            }
            
            // Check for file size (resumes are typically not too small or too large)
            const fileSizeKB = file.size / 1024;
            if (fileSizeKB > 50 && fileSizeKB < 500) {
                score += 5;
            }
            
            // Add variation based on file name patterns
            if (fileName.includes('resume') || fileName.includes('cv')) {
                score += 10; // Strong indicator of resume
            }
            
            // Add some randomness to make scores more varied
            score += Math.floor(Math.random() * 20) - 5; // Random between -5 and +15
            
            // Ensure score is within valid range
            score = Math.max(20, Math.min(score, 95));
            
            // Simulate section detection based on score
            const hasEducation = score > 30;
            const hasExperience = score > 40;
            const hasAchievements = score > 60;
            const hasSkills = score > 35;
            const hasContact = score > 25;
            
            // Set analysis text based on score
            let analysisText = '';
            let analysisPoints = '';
            
            if (score >= 80) {
                analysisText = 'Your resume appears to have a strong structure. For a more detailed analysis, please upload a text file.';
                analysisPoints = `
                    <li>Strengths: Likely well-structured with relevant content</li>
                    <li>Areas for improvement: Content organization and formatting</li>
                    <li>Keywords optimization: Unable to verify without text analysis</li>
                `;
            } else if (score >= 60) {
                analysisText = 'Your resume appears to have a good structure. For a more detailed analysis, please upload a text file.';
                analysisPoints = `
                    <li>Strengths: Basic resume format detected with relevant sections</li>
                    <li>Areas for improvement: Content organization and formatting</li>
                    <li>Keywords optimization: Unable to verify without text analysis</li>
                `;
            } else if (score >= 40) {
                analysisText = 'This document may be a resume but needs improvements. For a more detailed analysis, please upload a text file.';
                analysisPoints = `
                    <li>Missing essential resume sections</li>
                    <li>Consider restructuring with standard resume format</li>
                    <li>Include education, experience, and skills sections</li>
                `;
            } else {
                analysisText = 'This document does not appear to be a properly formatted resume. Please upload a text file for detailed analysis.';
                analysisPoints = `
                    <li>This document is not a resume</li>
                    <li>Please upload a proper resume file</li>
                    <li>Include education, experience, and skills sections</li>
                `;
            }
            
            // Store analysis results globally
            currentAnalysisResults = {
                score,
                hasEducation,
                hasExperience,
                hasAchievements,
                hasSkills,
                hasContact,
                isPoem: false,
                isNonResume: false,
                analysisText,
                analysisPoints,
                fileName: file.name,
                fileSize: file.size,
                fileType: file.type
            };
            
            // Update UI with analysis results
            updateResumeAnalysisUI();
        }
        
        // Updated updateResumeAnalysisUI function
        function updateResumeAnalysisUI() {
            if (!currentAnalysisResults) return;
            
            const { score, hasEducation, hasExperience, hasAchievements, hasSkills, hasContact, isPoem, isNonResume, analysisText, analysisPoints } = currentAnalysisResults;
            
            // Show score card
            resumeScoreCard.style.display = 'block';
            const scoreCircle = document.getElementById('resumeScoreCircle');
            scoreCircle.textContent = score;
            
            // Update score circle color based on score
            scoreCircle.className = 'score-circle';
            if (isNonResume) {
                scoreCircle.classList.add('score-poor');
            } else if (score >= 90) {
                scoreCircle.classList.add('score-excellent');
            } else if (score >= 80) {
                scoreCircle.classList.add('score-good');
            } else if (score >= 70) {
                scoreCircle.classList.add('score-average');
            } else {
                scoreCircle.classList.add('score-poor');
            }
            
            // Update analysis text
            const analysisTextElement = document.getElementById('resumeAnalysisText');
            const analysisPointsElement = document.getElementById('resumeAnalysisPoints');
            
            analysisTextElement.textContent = analysisText;
            analysisPointsElement.innerHTML = analysisPoints;
            
            // Update section analysis
            updateSectionAnalysis(educationAnalysis, hasEducation, 'Education');
            updateSectionAnalysis(experienceAnalysis, hasExperience, 'Experience');
            updateSectionAnalysis(achievementsAnalysis, hasAchievements, 'Achievements');
            updateSectionAnalysis(skillsAnalysis, hasSkills, 'Skills');
            updateSectionAnalysis(contactAnalysis, hasContact, 'Contact Info');
            
            // Update format analysis
            const formatValue = formatAnalysis.querySelector('.analysis-value');
            if (isNonResume) {
                formatAnalysis.className = 'analysis-item poor';
                formatValue.textContent = 'Not a resume';
            } else if (isPoem) {
                formatAnalysis.className = 'analysis-item poor';
                formatValue.textContent = 'Poem format';
            } else if (score >= 70) {
                formatAnalysis.className = 'analysis-item good';
                formatValue.textContent = 'Professional format';
            } else {
                formatAnalysis.className = 'analysis-item average';
                formatValue.textContent = 'Needs improvement';
            }
            
            // Reset upload area
            resumeUpload.innerHTML = `
                <i class="fas fa-cloud-upload-alt"></i>
                <h3>Drag & Drop Your Resume Here</h3>
                <p>Supported formats: PDF, DOC, DOCX, TXT (Max size: 5MB)</p>
                <button class="btn" style="margin-top: 15px;">Browse Files</button>
            `;
            
            // Hide progress bar
            progressContainer.style.display = 'none';
            
            // Show notification
            if (isNonResume) {
                showNotification('This document is not a resume. Please upload a resume file.', 'warning');
            } else {
                showNotification('Resume analyzed successfully!', 'success');
            }
        }
        
        // Updated generateRecommendations function
        function generateRecommendations(score, hasEducation, hasExperience, hasAchievements, hasSkills, hasContact, isPoem, isNonResume) {
            if (isNonResume) {
                return `
1. This document is not a resume.
2. Please upload a properly formatted resume document.
3. A good resume should include sections for education, experience, and skills.
4. Consider using a professional resume template or builder.
                `;
            }
            if (isPoem) {
                return `
1. This document appears to be a poem, not a resume.
2. Please upload a properly formatted resume document.
3. A good resume should include sections for education, experience, and skills.
4. Consider using a professional resume template or builder.
                `;
            }
            
            let recommendations = [];
            
            if (!hasEducation) {
                recommendations.push("Add an Education section with your degrees, certifications, and academic achievements.");
            }
            
            if (!hasExperience) {
                recommendations.push("Include an Experience section detailing your work history, internships, and relevant projects.");
            }
            
            if (!hasAchievements) {
                recommendations.push("Highlight your achievements and accomplishments with specific examples and metrics where possible.");
            }
            
            if (!hasSkills) {
                recommendations.push("Create a Skills section listing your technical and soft skills relevant to the jobs you're applying for.");
            }
            
            if (!hasContact) {
                recommendations.push("Ensure your contact information is clearly visible at the top of your resume.");
            }
            
            if (score < 70) {
                recommendations.push("Consider using a professional resume template to improve formatting and structure.");
                recommendations.push("Quantify your achievements with numbers and percentages where possible.");
                recommendations.push("Tailor your resume for each job application by including relevant keywords from the job description.");
            }
            
            if (recommendations.length === 0) {
                return "Your resume is well-structured! Consider getting feedback from a career counselor or mentor for further improvements.";
            }
            
            return recommendations.map((rec, index) => `${index + 1}. ${rec}`).join('\n');
        }
        
        // Helper function to detect resume sections with improved pattern matching
        function detectSection(content, keywords) {
            // Check for each keyword as a standalone word or as part of a section header
            for (const keyword of keywords) {
                // Create a regex pattern that matches the keyword as a whole word
                const pattern = new RegExp(`\\b${keyword}\\b`, 'i');
                
                // Check if the keyword exists in the content
                if (pattern.test(content)) {
                    return true;
                }
                
                // Also check for the keyword at the beginning of a line (common for section headers)
                const lineStartPattern = new RegExp(`^\\s*${keyword}\\b`, 'im');
                if (lineStartPattern.test(content)) {
                    return true;
                }
                
                // Check for the keyword followed by a colon (common in section headers)
                const colonPattern = new RegExp(`\\b${keyword}\\s*:\\s*`, 'im');
                if (colonPattern.test(content)) {
                    return true;
                }
            }
            
            return false;
        }
        
        // Helper function to check for resume-specific patterns
        function checkResumePatterns(content) {
            // Check for common resume section headers
            const sectionPatterns = [
                /\b(education|academic|qualification)\b.*\n/i,
                /\b(experience|employment|work history|professional)\b.*\n/i,
                /\b(skills|expertise|competencies|technical)\b.*\n/i,
                /\b(achievement|accomplishment|award|honor)\b.*\n/i,
                /\b(contact|information|profile|details)\b.*\n/i
            ];
            
            // Check for date patterns (common in resumes)
            const datePatterns = [
                /\b(19|20)\d{2}\s*-\s*(19|20)\d{2}\b/, // Year ranges
                /\b(jan|feb|mar|apr|may|jun|jul|aug|sep|oct|nov|dec)[a-z]*\s+\d{4}\b/i, // Month Year
                /\b\d{1,2}\/\d{1,2}\/\d{2,4}\b/ // Date formats
            ];
            
            const sectionMatches = sectionPatterns.filter(pattern => pattern.test(content)).length;
            const dateMatches = datePatterns.filter(pattern => pattern.test(content)).length;
            
            // Consider it a resume if it has at least 2 section patterns or 1 section and 2 date patterns
            return sectionMatches >= 2 || (sectionMatches >= 1 && dateMatches >= 2);
        }
        
        // Function to update section analysis
        function updateSectionAnalysis(element, hasSection, sectionName) {
            const valueElement = element.querySelector('.analysis-value');
            
            if (hasSection) {
                element.className = 'analysis-item excellent';
                valueElement.textContent = 'Detected';
            } else {
                element.className = 'analysis-item poor';
                valueElement.textContent = 'Not detected';
            }
        }
        
        // Updated download report button event listener
        downloadReportBtn.addEventListener('click', () => {
            if (!currentAnalysisResults) {
                showNotification('No analysis results available', 'error');
                return;
            }
            
            const { score, hasEducation, hasExperience, hasAchievements, hasSkills, hasContact, isPoem, isNonResume, analysisText, analysisPoints, fileName, fileSize, fileType } = currentAnalysisResults;
            
            // Create report content
            const reportContent = `
SMART HIRE AI - RESUME ANALYSIS REPORT
==========================================
File Information:
- File Name: ${fileName}
- File Type: ${fileType}
- File Size: ${Math.round(fileSize / 1024)} KB
- Analysis Date: ${new Date().toLocaleDateString()}
OVERALL SCORE: ${score}/100
${isNonResume ? 'NOT A RESUME' : score >= 90 ? 'EXCELLENT' : score >= 80 ? 'GOOD' : score >= 70 ? 'AVERAGE' : score >= 50 ? 'BELOW AVERAGE' : 'POOR'}
SUMMARY:
${analysisText}
DETAILED ANALYSIS:
${analysisPoints.replace(/<li>/g, '- ').replace(/<\/li>/g, '\n')}
SECTION DETECTION:
- Education: ${hasEducation ? 'Detected ✓' : 'Not detected ✗'}
- Experience: ${hasExperience ? 'Detected ✓' : 'Not detected ✗'}
- Achievements: ${hasAchievements ? 'Detected ✓' : 'Not detected ✗'}
- Skills: ${hasSkills ? 'Detected ✓' : 'Not detected ✗'}
- Contact Information: ${hasContact ? 'Detected ✓' : 'Not detected ✗'}
- Format: ${isNonResume ? 'Not a resume' : isPoem ? 'Poem format (not a resume)' : score >= 70 ? 'Professional format' : 'Needs improvement'}
RECOMMENDATIONS:
${generateRecommendations(score, hasEducation, hasExperience, hasAchievements, hasSkills, hasContact, isPoem, isNonResume)}
==========================================
This report was generated automatically by Smart Hire AI.
For questions or concerns, please contact support@smarthireai.com
            `;
            
            // Create a blob and download
            const blob = new Blob([reportContent], { type: 'text/plain' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `Resume_Analysis_Report_${fileName.replace(/\.[^/.]+$/, '')}_${new Date().toISOString().split('T')[0]}.txt`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            
            showNotification('Report downloaded successfully!', 'success');
        });
        
        // Company dashboard functionality
        document.addEventListener('DOMContentLoaded', function() {
            // Add event listeners for "View Candidates" buttons
            const viewCandidatesButtons = document.querySelectorAll('.job-actions .btn-sm');
            viewCandidatesButtons.forEach(button => {
                button.addEventListener('click', function() {
                    const jobCard = this.closest('.job-card');
                    const candidatesList = jobCard.querySelector('.candidates-list');
                    
                    if (candidatesList.style.display === 'none' || !candidatesList.style.display) {
                        candidatesList.style.display = 'block';
                        this.textContent = 'Hide Candidates';
                    } else {
                        candidatesList.style.display = 'none';
                        this.textContent = 'View Candidates';
                    }
                });
            });
        });
        
        // Notification function
        function showNotification(message, type = 'success') {
            const notificationEl = document.getElementById('notification');
            const notificationMessage = notificationEl.querySelector('.notification-message');
            const notificationIcon = notificationEl.querySelector('.notification-icon');
            
            // Update message
            notificationMessage.textContent = message;
            
            // Update icon and color based on type
            notificationEl.className = 'notification';
            if (type === 'success') {
                notificationEl.classList.add('notification-success');
                notificationIcon.className = 'notification-icon fas fa-check-circle';
            } else if (type === 'error') {
                notificationEl.classList.add('notification-error');
                notificationIcon.className = 'notification-icon fas fa-exclamation-circle';
            } else if (type === 'info') {
                notificationEl.classList.add('notification-info');
                notificationIcon.className = 'notification-icon fas fa-info-circle';
            } else if (type === 'warning') {
                notificationEl.classList.add('notification-warning');
                notificationIcon.className = 'notification-icon fas fa-exclamation-triangle';
            }
            
            // Show notification
            notificationEl.classList.add('show');
            
            // Hide after 3 seconds
            setTimeout(() => {
                notificationEl.classList.remove('show');
            }, 3000);
        }
        
        // Jotform Chatbot Script
        const jfAgentCacheName = 'dynamic-agent-v1';

        const sanitizeVariables = (url, width, height) => {
          try {
            const sanitizedUrl = new URL(url);
            const url = sanitizedUrl.toString();
            const width = parseInt(width);
            const height = parseInt(height);
            return { url, width, height };
          } catch (e) {
            console.error('Error sanitizing variables', e);
            return { url: '', width: 0, height: 0 };
          }
        };

        const handlePictureInPictureRequest = async event => {
          if (event.data.type !== 'jf-request-pip-window') {
            return;
          }
          const { _url, _width, _height } = event.data;
          const { url, width, height } = sanitizeVariables(_url, _width, _height);
          if (url === '' || width === 0 || height === 0) {
            return;
          }
          if ('documentPictureInPicture' in window) {
            // return if already in picture in picture mode
            if (window.documentPictureInPicture.window) {
              return;
            }
            const pipWindow = await window.documentPictureInPicture.requestWindow({
              width,
              height,
              disallowReturnToOpener: true
            });
            // copy styles from main window to pip window
            [...document.styleSheets].forEach(styleSheet => {
              try {
                const cssRules = [...styleSheet.cssRules]
                  .map(rule => rule.cssText)
                  .join('');
                const style = document.createElement('style');
                style.textContent = cssRules;
                pipWindow.document.head.appendChild(style);
              } catch (e) {
                const link = document.createElement('link');
                link.rel = 'stylesheet';
                link.type = styleSheet.type;
                link.media = styleSheet.media;
                link.href = styleSheet.href;
                pipWindow.document.head.appendChild(link);
              }
            });
            pipWindow.document.body.innerHTML = `<iframe src="${url}" style="width: ${width}px; height: ${height}px;" allow="microphone *; display-capture *;"></iframe>`;
            return { success: true, isActive: false };
          }
        };

        window.addEventListener('message', handlePictureInPictureRequest);

        // Initialize Jotform Agent
        (function() {
          const src = "https://www.jotform.com/s/umd/2a1c0e54014/for-embedded-agent.js";
          const script = document.createElement('script');
          script.src = src;
          script.async = true;
          script.onload = function() {
            if (typeof window.AgentInitializer !== 'undefined') {
              window.AgentInitializer.init({
                agentRenderURL: "https://www.jotform.com/agent/0199381c5acf787eb21b619f1e40f5b22b9d",
                rootId: "JotformAgent-0199381c5acf787eb21b619f1e40f5b22b9d",
                formID: "0199381c5acf787eb21b619f1e40f5b22b9d",
                contextID: "01995c140abc75fbbc2f84af198fd053362e",
                initialContext: "",
                queryParams: ["skipWelcome=1","maximizable=1"],
                domain: "https://www.jotform.com",
                isDraggable: false,
                background: "linear-gradient(180deg, #0E408A 0%, #0E408A 100%)",
                buttonBackgroundColor: "#051258",
                buttonIconColor: "#FFFFFF",
                inputTextColor: "#481414",
                variant: false,
                customizations: {"greeting":"Yes","greetingMessage":"Hi! How can I assist you?","openByDefault":"No","pulse":"Yes","position":"left","autoOpenChatIn":"1","layout":"extended"},
                isVoice: false,
                isVoiceWebCallEnabled: true
              });
            }
          };
          document.head.appendChild(script);
        })();
        
        // Add event listener to the "Try Chatbot" button
        document.addEventListener('DOMContentLoaded', function() {
            const tryChatbotBtn = document.getElementById('tryChatbotBtn');
            if (tryChatbotBtn) {
                tryChatbotBtn.addEventListener('click', function() {
                    // Try to open the chatbot
                    if (typeof window.JotformAgent !== 'undefined') {
                        window.JotformAgent.open();
                    } else {
                        showNotification('Chatbot is loading. Please try again in a moment.', 'info');
                    }
                });
            }
        });
    </script>
</body>
</html>
