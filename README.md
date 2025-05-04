# Local Deep Research

A data analysis and research project environment.

## Development Environment

This project is set up to use GitHub Codespaces, so you can just run the LLM and not worry about your local environment getting f'd up.  Be sure to open this project 'within a codespace' locally or remote.

### Using GitHub Codespaces

1. Click the "Code" button on the GitHub repository
2. Select "Create codespace on main"
3. Wait for the codespace to be created and initialized

The codespace will automatically:

- Set up a Python 3.11 environment
- Install all required dependencies from `requirements.txt`
- Configure VS Code with useful extensions for data analysis

## Setup

Sample data is available at https://github.com/JannikArndt/PostgreSQLSampleDatabase/tree/master

Run the following command to start the MCP server:

```
docker run -it -p 8000:8000 \
  -e DATABASE_URI=postgresql://evan@localhost:5432/bun \
  crystaldba/postgres-mcp --access-mode=unrestricted --transport=sse
```
