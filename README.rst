
Sample Flow to execute
============
Hi
I want to book a hotel room?
What is the starting price for the Standard Room?
Ok, book standard room for me.
bye

Installation
============


.. code-block:: sh

   $ pip3 install rasa
   $ pip3 install rasa_sdk

the language model with:

.. code-block:: sh

   $ pip3 install rasa[spacy]
   $ python3 -m spacy download en_core_web_md
   $ python3 -m spacy link en_core_web_md en

and the Fetchable Python client-side SDK with:

.. code-block:: sh

   $ pip3 install fetchable

You'll also need to sign up for a Fetchable account, download your API keys and export an environment variable with the absolute path to the file containing them with:

.. code-block:: sh

   $ export FETCHABLE_AUTH_FILE=/path/to/fetchable_auth_keys.json

Running
=======

Assuming you have the requirements installed - if you would like to run the code without going through the tutorial and building it from scratch run the following commands:

1. Train the chatbot:

.. code-block:: sh

   $ rasa train

2. Launch the action server:

.. code-block:: sh

   $ rasa run actions

3. Launch the chatbot in a different terminal:

.. code-block:: sh

   $ rasa shell --endpoint endpoints.yml


Files
=====

| workspace
| ├── data
| │   ├── nlu.md
| │   └── stories.md
| ├── __init__.py
| ├── .gitignore
| ├── actions.py
| ├── config.yml
| ├── credentials.yml
| ├── domain.yml
| ├── endpoints.yml
| ├── LICENCE
| └── README.rst
| └── requirements.txt
