# Weather Query MCP Server/Client Example

This project is a weather query client that interacts with an MCP (Model-Client-Protocol) server to fetch and display weather information for a specified city.

## Features

- Connects to an MCP server to list available tools.
- Queries weather information for a specified city.
- Displays formatted weather information including temperature, humidity, wind speed, and weather description.

## Requirements

- Python 3.8+
- `openai` library
- `dotenv` library
- `mcp` library

## Setup

1. Clone the repository:
    ```sh
    git clone <repository_url>
    cd <repository_directory>
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv .venv
    source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Create a `.env` file in the root directory and add your OpenAI API key and other configurations:
    ```env
    OPENAI_API_KEY=<your_openai_api_key>
    BASE_URL=<your_base_url>
    MODEL=<your_model>
    ```

## Usage

1. Start the MCP server:
    ```sh
    python server.py
    ```

2. Run the client and connect to the server:
    ```sh
    python client.py <path_to_server_script>
    ```

3. Interact with the client:
    - Type the name of the city in English to get the weather information.
    - Type `quit` to exit the client.

## Project Structure

- `server.py`: Contains the MCP server implementation and weather query tool.
- `client.py`: Contains the MCP client implementation to interact with the server.
- `.env`: Environment variables for API keys and configurations.
- `.gitignore`: Specifies files and directories to be ignored by git.
- `README.md`: Project documentation.

## License

This project is licensed under the MIT License.