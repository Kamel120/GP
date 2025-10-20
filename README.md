# MyProject

A modern Django web application featuring a responsive design, user authentication, and a dynamic light/dark mode theme switcher.

## Features

- **User Authentication**: Secure login and logout functionality for users.
- **Dynamic Theme Switching**: A beautiful theme switcher in the navigation bar allows users to toggle between light and dark modes. The user's preference is saved in their browser for a consistent experience.
- **Social Authentication**: Convenient "Login with Google" feature powered by `django-allauth`.
- **Responsive Design**: Built with Bootstrap 5, the interface is fully responsive and looks great on all devices, from desktops to mobile phones.
- **Theme-Aware Components**: All major components, including the navigation bar, hero section, and content cards, adapt their styling for both light and dark modes.
- **Static Pages**: Utilizes Django's `flatpages` app to easily manage static content like an "About Us" page.
- **Improved Developer Experience**: The underlying Pygments library has been enhanced to automatically detect dark terminal backgrounds, providing better syntax highlighting in the console.

## Screenshots

Here's a glimpse of the application in both light and dark modes.

**Light Mode**

!Light Mode Screenshot

**Dark Mode**

!Dark Mode Screenshot

_(Note: You will need to add your own screenshots named `screenshot-light.png` and `screenshot-dark.png` to the project's root directory.)_

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Python 3.8+
- Pip

### Installation

1.  **Clone the repository:**

    ```sh
    git clone <your-repository-url>
    cd GP
    ```

2.  **Create and activate a virtual environment:**

    ```sh
    # For Windows
    python -m venv venv
    venv\Scripts\activate

    # For macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Install the required dependencies:**
    The project relies on several packages. You can install them directly:

    ```sh
    pip install django django-allauth requests requests-oauthlib PyJWT cryptography
    ```

    Alternatively, if you have a `requirements.txt` file:

    ```sh
    pip install -r requirements.txt
    ```

    _(Note: You can create an up-to-date `requirements.txt` file with `pip freeze > requirements.txt` after installing the packages.)_

4.  **Apply database migrations:**

    ```sh
    python myproject/manage.py migrate
    ```

5.  **Create a superuser to access the admin panel:**

    ```sh
    python myproject/manage.py createsuperuser
    ```

6.  **Run the development server:**
    ```sh
    python myproject/manage.py runserver
    ```

The application will be available at `http://127.0.0.1:8000/`.

## Technologies Used

- **Backend**: Python, Django
- **Frontend**: HTML, CSS, JavaScript, Bootstrap 5, `django-allauth`
- **Syntax Highlighting**: Pygments
