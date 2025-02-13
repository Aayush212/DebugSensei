# DebugSensei
This project is a Chat Assistant built using Gradio as the frontend and the DebugSensei model for generating responses. The assistant takes user prompts, maintains a conversation history, and provides relevant responses based on the context.

## Features
> Interactive Chat Interface using Gradio

> Utilizes DebugSensei model for generating responses

> Maintains conversation history for context-aware responses

> Easy-to-use web interface

## Tech Stack
> Python: Core programming language

> Gradio: Frontend UI for chat interface

## Python Packages:
  ```gradio```

  ```requests```

## Installation
1. Clone the Repository:
    ```
    git clone https://github.com/Aayush212/DebugSensei.git
    cd DebugSensei
    ```

2. Create a Virtual Environment:
    ```
    python -m venv venv
    ```

3. Activate the Virtual Environment:
   > On Windows:
   
         venv\Scripts\activate

   > On macOS/Linux:
   
         source venv/bin/activate

5. Install the Required Packages:
     ```
     pip install -r requirements.txt
     ```

## Running the Application
  ```python app.py```

After running, the Gradio interface will be available at:
  ```http://127.0.0.1:7860```

## Usage
1. Enter your prompt in the input box.
2. The assistant will maintain a conversation history and generate a response using the DebugSensei model.
3. The conversation history allows for context-aware replies.

## Code Explanation
```generate_response(prompt)```:
    Function that takes the user prompt, appends it to the conversation history, and makes 
    a POST request to the DebugSensei model API.

```interface = gr.Interface(...)```:
    Gradio interface setup with input and output components.

```interface.launch()```:
    Launches the Gradio web interface.

## API Endpoint

The application communicates with the DebugSensei model through the following endpoint:

  ```
  http://localhost:11434/api/generate
  ```

Ensure that the DebugSensei model is running locally on port 11434.

## Example Request
  ```
  {
      "model": "DebugSensei",
      "prompt": "Hello, how can I help you today?",
      "stream": false
  }
  ```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.

2. Create a new branch:
  ```
  git checkout -b feature-name
  ```

4. Make your changes and commit:
  ```
  git commit -m "Add feature-name"
  ```

4. Push to your fork:
  ```
  git push origin feature-name
  ```
5. Create a pull request.

## License

This project is licensed under the MIT License.

## Contact
For any questions or feedback, feel free to reach out:

Mail - ```maayush410@gmail.com```

GitHub - ```github.com/Aayush212```

## Troubleshooting

> Ensure that the DebugSensei model is running on the specified port.

> If facing CORS issues, configure your local server settings.

> For environment-related issues, make sure to activate the virtual environment.

## To Do

> Add support for more models.

> Implement conversation reset functionality.

> Enhance UI with more customization options.

## Changelog

```v1.0.0``` : Initial release with basic chat functionality.



