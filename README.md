1) manage.py:
    - We are installing many different libraries.
    - We are then creating an object cli from the class Flaskgroup.
2) __init__.py:
    - We have created functions to create the app, find bad requests, find errors and handle them.
    - We have created a SQLAlchemy() and a Migrate() object.
3) views.py:
    - We are importing the necessary libraries.
    - We are then creating a views object from the Blueprints class.
    - We have then created functions for: login, dashboard, profile, order, help_page and editor.
4) api.py:
    - We are creating and api for the app.
    - We have imported the necessary libraries.
    - We have like before created an object for Blueprint class.
    - We have then created a login() function which checks for both the email and password of the user.
    - We have then created a function add_address() to find the house number, city, state, country, pin code etc.
    - We have also created the function create_order() to create the order by using the users email, their query, the user, the product id and the amount.
5) models.py:
    - Address.py adds the address_obj into a session, this includes the users house number, city, state, country, pin code etc.
    - Orders.py adds the order_obj into a session, this includes the users email, their query, the user, the product id and the amount.
    - Products.py is a database for each of the products and thier info which includes name, image, rating, marked_price, selling_price.
    - Tickets.py is the reciept of the order the user has just made.
    - Users.py is the database for all of the users info this also includes the address, orders and tickets.
