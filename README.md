# MedBot

By combining advanced technology with medical knowledge, we aim to create a powerful tool that empowers users and promotes health awareness. Through its two-phase approach, MediBot assists users in understanding their symptoms, identifying potential diseases, and offering guidance on prevention methods.

In the first phase, MediBot assumes that the user already knows the name of disease they have been diagnosed with and desires to gain further insights. It caters to their needs by providing a comprehensive disease description, outlining the causes behind the condition, and offering preventive measures. By interacting with the bot, users can acquire accurate and reliable information regarding their diagnosed disease.

Moving into the second phase, MediBot engages users by prompting them to input their symptoms. Based on this input, the chatbot analyzes the data and matches it against its extensive database of diseases and symptoms. Subsequently, MediBot provides users with the name of the disease that corresponds to their symptoms, along with additional symptoms that individuals may encounter when affected by that particular disease.

This unique approach assists users in gaining further confidence and certainty about their health conditions. By reading the chatbot's responses and discovering that they are experiencing additional symptoms associated with the disease, users can strengthen their understanding and awareness of their own medical condition. This empowers individuals to make informed decisions regarding their health, seek appropriate medical attention, and take necessary precautions.


## Table of Contents

- [Actions](#actions)
- [Data](#data)
- [Tests](#tests)
- [Configuration](#configuration)
- [Credentials](#credentials)
- [Domain](#domain)
- [Endpoints](#endpoints)
- [README](#readme)

## Actions

The `actions` directory contains custom action files for the Rasa chatbot. These files define custom actions that the chatbot can perform.

## Data

The `data` directory contains training data for the Rasa chatbot. This includes NLU training data and stories for dialogue management.

## Tests

The `tests` directory contains test cases for the Rasa chatbot. These tests ensure that the chatbot behaves as expected in different scenarios.

## Configuration

The `config.yml` file contains the configuration settings for the Rasa chatbot. This includes pipeline configuration for natural language understanding (NLU) and dialogue management.

## Credentials

The `credentials.yml` file contains credentials for external services used by the Rasa chatbot. This may include credentials for APIs or databases.

## Domain

The `domain.yml` file defines the domain of the Rasa chatbot. It includes intents, entities, actions, responses, and templates used by the chatbot.

## Endpoints

The `endpoints.yml` file specifies the endpoints for the Rasa chatbot. This includes endpoints for connecting to external services such as a tracker store or event broker.

## README

The `README.md` file provides information about the Rasa chatbot project, its structure, and how to use and contribute to it.



# Install dependencies

Run:
`pip install -r requirements.txt`

# Run the bot
Use `rasa train` to train a model.

Then to talk to the bot, run:

`rasa shell --debug`

Note that --debug mode will produce a lot of output meant to help you understand how the bot is working under the hood. To simply talk to the bot, you can remove this flag.

# Overview of the files

data/nlu.yml - contains NLU training data

data/rules.yml - contains rules training data

data/stories*.yml - contains stories training data

actions/actions.py - contains custom action/api code

domain.yml - the domain file, including bot response templates

config.yml - training configurations for the NLU pipeline and policy ensemble

tests/ - end-to-end tests
