# YouTube Clone

A high-performance, modular YouTube clone built with **Django 6.0** and **Python 3.13**. This project demonstrates modern web architecture, utilizing `uv` for lightning-fast dependency management and `ImageKit.io` for cloud-based media processing.

## 🚀 Features

- **User Authentication:** Fully implemented registration, login, and logout workflows.
- **Video Management:** (In Progress) Foundation for video uploads, metadata tracking (views, likes, dislikes), and cloud integration.
- **Cloud Media:** Integrated with `ImageKit.io` for optimized video and image delivery.
- **Modern Stack:** Built on the latest Django 6.0 standards for long-term stability and security.

## 🛠️ Technical Stack

- **Backend:** Python 3.13, Django 6.0
- **Database:** SQLite (Development)
- **Dependency Management:** [uv](https://github.com/astral-sh/uv)
- **Media Hosting:** ImageKit.io
- **Environment:** `python-dotenv` for configuration management

## 📦 Installation & Setup

This project uses `uv` for dependency management. If you don't have it installed, get it via `curl -LsSf https://astral.sh/uv/install.sh | sh`.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dimipash/YouTube-Clone.git
   cd YouTube-Clone
   ```

2. **Set up the virtual environment and install dependencies:**
   ```bash
   uv sync
   ```

3. **Configure Environment Variables:**
   Copy the sample environment file and fill in your credentials (especially ImageKit keys):
   ```bash
   cp youtube/.env.sample youtube/.env
   ```

4. **Run Migrations:**
   ```bash
   cd youtube
   uv run manage.py migrate
   ```

5. **Start the Development Server:**
   ```bash
   uv run manage.py runserver
   ```

## 🏗️ Project Structure

- `youtube/`: Main Django project configuration.
- `accounts/`: User management, profiles, and authentication logic.
- `videos/`: Core business logic for video content, metadata, and interactions.
- `templates/`: Global and app-specific HTML templates.

## 🗺️ Roadmap

- [ ] Implementation of video upload views and forms.
- [ ] Video playback page with comments section.
- [ ] User profiles and channel customization.
- [ ] Search functionality and filtering.
- [ ] Real-time notifications for likes/subscriptions.

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.
