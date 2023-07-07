# `LibraIO`

Bookstore with filtering and search for books of interest. Also provides the ability to add and send book deletion requests to *authorized users*.
___
## Functionality
- Open book list [**BookListView**](https://github.com/Segfaul/libraio/blob/fbda70819b09165a13bda165ce84f51478db227f/libraio/books/views.py#L14-L23)
- Adding a book to the general list [**AddBookView**](https://github.com/Segfaul/libraio/blob/fbda70819b09165a13bda165ce84f51478db227f/libraio/books/views.py#L36-L54)
- Sending book deletion request [**DeleteReqView**](https://github.com/Segfaul/libraio/blob/fbda70819b09165a13bda165ce84f51478db227f/libraio/books/views.py#L117-L135)
- Filtering books by genre [**BookGenreView**](https://github.com/Segfaul/libraio/blob/fbda70819b09165a13bda165ce84f51478db227f/libraio/books/views.py#L151-L163)
- Searching for the desired book by author/genre [**BookSearchView**](https://github.com/Segfaul/libraio/blob/fbda70819b09165a13bda165ce84f51478db227f/libraio/books/views.py#L166-L181)

## Technologies and Frameworks
- Python 3.11 
- Django 4.2
- HTML, CSS, JS, Jquery[AJAX]
- SQLite 3

___

## Installation

1. Clone the repository to the local machine

    ```shell
    git clone https://github.com/Segfaul/libraio.git
    ```

2. Go to the repository directory

    ```shell
    cd RKSP
    ```

3. Create and activate a virtual environment

    ```shell
    python -m venv env
    source env/bin/activate
    ```
4. Set project dependencies

    ```python
    pip install -r requirements.txt
    ```

4. Go to the libraio directory

    ```shell
    cd libraio
    ```

5. Create database migrations and apply them

    ```python
    python manage.py makemigrations
    python manage.py migrate
    ```

6. Create a Django project superuser (admin)

    ```python
    python manage.py createsuperuser
    ```

7. Run the project on localhost in the background

    ```python
    python manage.py runserver &
    ```

8. Go to the site and enter the previously created data of the superuser (step 6)

    ```shell
    http://127.0.0.1:8000
    ```

## Settings

[Migrations](https://docs.djangoproject.com/en/4.2/topics/migrations/) - - is Django's way of propagating changes you make to your models (adding a field, removing a model, etc.) to the database schema.

1. Create new migrations based on the changes you made to your models

    ```python
    python manage.py makemigrations
    ```

2. Using previously created migrations

    ```python
    python manage.py migrate
    ```

___
