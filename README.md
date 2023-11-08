# telegram_bot
telegram-bot


-main.py - Entry point, the code to start the bot and initialize all other modules.
-config.py - A file containing all configuration parameters, such as the bot token and database connection data. Storing settings in a Python file is not the best practice, but it is the simplest way. Settings can also be stored in environment variables or special files (e.g., INI, JSON), and --config.py can serve as an abstraction of data. However, in this bot, the simplest method will be used.
-db.py - Functions for connecting to and working with the database. This file will serve as an abstraction of the database from the main code.
-text.py - All texts used by the bot. This file will contain all greetings, error messages, and other textual data for the bot. Storing text in a Python file is not the best practice since text changes can only be made through code. However, texts change infrequently (often never), so we'll go with the simplest approach again.
-kb.py - All keyboards used by the bot. This file will contain all keyboards, both static and dynamically generated using functions.
-middlewares.py - The name of the file speaks for itself. This file will contain all used middlewares (there will be only two).
-states.py - It will store auxiliary classes for the Finite State Machine (FSM) and factories for Callback Data for Inline keyboard buttons.
-utils.py - Various functions. This file will contain functions for broadcasting, text and image generation through APIs, and others.
-handlers.py - The main file, which will contain almost all the bot's code. It will consist of handler functions with decorators (filters).
-admin.py - Event handlers, keyboards, classes, and all other code for the bot's admin interface. Again, if you follow best practices, it would be better to separate this into a separate folder and create modules for keyboards, texts, handlers, and everything else. Our admin functionality will have basic functionality, so we will implement everything in one file.
