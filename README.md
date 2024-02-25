# MedBot

By combining advanced technology with medical knowledge, we aim to create a powerful tool that empowers users and promotes health awareness. Through its two-phase approach, MediBot assists users in understanding their symptoms, identifying potential diseases, and offering guidance on prevention methods.

In the first phase, MediBot assumes that the user already knows the name of disease they have been diagnosed with and desires to gain further insights. It caters to their needs by providing a comprehensive disease description, outlining the causes behind the condition, and offering preventive measures. By interacting with the bot, users can acquire accurate and reliable information regarding their diagnosed disease.

Moving into the second phase, MediBot engages users by prompting them to input their symptoms. Based on this input, the chatbot analyzes the data and matches it against its extensive database of diseases and symptoms. Subsequently, MediBot provides users with the name of the disease that corresponds to their symptoms, along with additional symptoms that individuals may encounter when affected by that particular disease.

This unique approach assists users in gaining further confidence and certainty about their health conditions. By reading the chatbot's responses and discovering that they are experiencing additional symptoms associated with the disease, users can strengthen their understanding and awareness of their own medical condition. This empowers individuals to make informed decisions regarding their health, seek appropriate medical attention, and take necessary precautions.

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
