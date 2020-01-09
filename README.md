# Cookiecutter Chatbot

_A logical, reasonably standardized, but flexible project structure for doing and sharing chatbot related work.


### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.6
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

### To start a new project, run:
------------

    cookiecutter https://github.com/drivendata/cookiecutter-data-science


[![asciicast](https://asciinema.org/a/244658.svg)](https://asciinema.org/a/244658)


### The resulting directory structure
------------

The directory structure of your new project looks like this: 

```
    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── english ── nlu.md      <- Training data for english bot
    │   ├── hindi ── nlu.md        <- Training data for hindi bot
    │   ├── marathi ── nlu.md      <- Training data for marathi bot
    │   └── gujrati ── nlu.md       <- Training data for gujrati bot
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── references         <- other explanatory materials.
    │
    ├── model               <- nlu model and core model
    │
    ├── actions.py           <- code for your custom actions like booking a calendar, query a database etc.
    │
    ├── stories.md           <- stories which decide the flow of your chatbot
    │
    ├── endpoints.yml        <- details for connecting to channels like fb messenger
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    ├── src                <- Source code for use in this project.
    │   ├── english ── domain.yml    <- your assistant’s domain for the english chatbot
    │   │           ── config.yml    <- configuration of your NLU and Core models for the english chatbot
    │   │
    │   │── hindi ── domain.yml    <- your assistant’s domain for the hindi chatbot
    │   │         ── config.yml    <- configuration of your NLU and Core models for the hindi chatbot
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.testrun.org
```

## Contributing

We welcome contributions! [See the docs for guidelines](https://drivendata.github.io/cookiecutter-data-science/#contributing).

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests
