# LAUNCHR

A minimal  Gitlab CI Task Launcher powered by Python and Flask.

* What is LaunchR? 

      A { python, flask, sqlite } powered tiny little Gitlab CI task runner.

* How do I use it?

      1. edit the configuration in the launchr.py file or
         export an LAUNCHR_SETTINGS environment variable
         pointing to a configuration file.

      2. install the app from the root of the project directory

         pip install --editable .

      3. Instruct flask to use the right application 

         LINUX:
           export FLASK_APP=launchr.launchr
         WINDOWS:
           set FLASK_APP=launchr.launchr

      4. initialize the database with this command:

         flask initdb

      5. now you can run launchr:

         flask run

         the application will greet you on
         http://localhost:5000/

* Are there unit tests?

      You betcha.  Run `python setup.py test` to see
      the tests pass.
