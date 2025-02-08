
# Django Tutorial Project

This is a Django project created as part of a tutorial to learn the basics of Django web development.

## Getting Started

These instructions will help you set up and run the project on your local machine for development and testing purposes.

### Prerequisites

- Python 3.x
- Django 3.x
- pip (Python package installer)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Maxidonx/Django-poll.git
    cd djangotutorial
    ```

2. Create a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

4. Apply migrations:
    ```bash
    python manage.py migrate
    ```

5. Run the development server:
    ```bash
    python manage.py runserver
    ```

6. Open your browser and navigate to `http://127.0.0.1:8000/` to see the project in action.

## Project Structure

- `djangotutorial/` - Main project directory
- `manage.py` - Command-line utility for administrative tasks
- `app_name/` - Replace with your app's name, contains the app's code

## Contributing

Feel free to submit pull requests or open issues to improve this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Django documentation
- Any other resources or tutorials you followed


============
django-polls
============

django-polls is a Django app to conduct web-based polls. For each
question, visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "polls" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...,
        "django_polls",
    ]

2. Include the polls URLconf in your project urls.py like this::

    path("polls/", include("django_polls.urls")),

3. Run ``python manage.py migrate`` to create the models.

4. Start the development server and visit the admin to create a poll.

5. Visit the ``/polls/`` URL to participate in the poll.