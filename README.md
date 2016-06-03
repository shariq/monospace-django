## Monospace

Monospace is a social network for developers. It's our sample Django
application, showing how to use Stripe to charge subscribers.

Monospace uses the Stripe Javascript bindings to validate a credit card, and
the Stripe Python bindings to create a customer and add the credit card to that
customer. Customers can also update their credit card.

## Installation steps

You will need a publishable token and a secret token. Add them both to
monospace/settings.py

Install virtualenv if you don't already have it:

    easy_install virtualenv

Run the following commands from the root of this project:

    virtualenv --no-site-packages env
    source env/bin/activate
    pip install -r requirements.txt
    python monospace/manage.py syncdb
    python monospace/manage.py runserver
