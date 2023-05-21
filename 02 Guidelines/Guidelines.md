Prompting Principles

Principle 1: Write clear and specific instructions

Tactic 1: Use delimiters to clearly indicate distinct parts of the input
Delimiters can be anything like: ```, """, < >, <tag> </tag>
Tactic 2: Ask for a structured output
JSON, HTML
Tactic 3: Ask the model to check whether conditions are satisfied
Tactic 4: "Few-shot" prompting

Principle 2: Give the model time to “think”

Tactic 1: Specify the steps required to complete a task
and you can ask for output in a specified format
Tactic 2: Instruct the model to work out its own solution before rushing to a conclusion
Note that the student's solution is actually not correct.
We can fix this by instructing the model to work out its own solution first.

Model Limitations: Hallucinations
Boie is a real company, the product name is not real.
Notes on using the OpenAI API outside of this classroom
To install the OpenAI Python library:

!pip install openai
The library needs to be configured with your account's secret key, which is available on the website.

You can either set it as the OPENAI_API_KEY environment variable before using the library:

 !export OPENAI_API_KEY='sk-...'
Or, set openai.api_key to its value:

import openai
openai.api_key = "sk-..."

A note about the backslash

In the course, we are using a backslash \ to make the text fit on the screen without inserting newline '\n' characters.
GPT-3 isn't really affected whether you insert newline characters or not. But when working with LLMs in general, you may consider whether newline characters in your prompt may affect the model's performance.