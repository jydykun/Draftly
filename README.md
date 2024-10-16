# Draftly
A minimal blog engine built with Flask, styled with Tailwind CSS, and powered by TinyMCE. Work in progress...

## Overview
Draftly is a beginner-friendly blog engine designed for simplicity. It allows users to create and manage posts with categories (no tags) through a dashboard. The project uses Flask on the backend, with a focus on delivering clean designs using Tailwind CSS and dynamic post editing with TinyMCE.

## Features
- Post Management: Create, update, and delete posts with category support.
- Dashboard Interface: Manage your content easily from an admin dashboard.
- TinyMCE Editor: Rich text editor for creating engaging blog posts.
- Tailwind CSS Styling: Responsive design with minimal custom CSS.
- Blueprints in Flask: Clean structure with modular routes and views.
- SQLite Database: Simple, lightweight database for managing content.
- Still Under Construction: Some features are being finalized!

## Installation & Setup

1. Clone the repository
```bash
git clone https://github.com/yourusername/draftly.git
cd draftly
```

2. Set up a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install Dependencies
```bash
pip install -r requirements.txt
```

4. Initialize Database
```bash
python cli.py init-db
```

5. Run the Development Server
```bash
python cli.py run-debug
```

## Deployment
4. Using Render:
- Configure the Start Command:
```bash
gunicorn wsgi:app
```
- Ensure environment variables are properly set (e.g., FLASK_ENV).
- Optionally, use persistent volumes on Render to store your SQLite database.