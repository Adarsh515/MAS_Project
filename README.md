# MAS_Project

## Overview

MAS_Project is an AI Multi-Agent System (MAS) architecture designed to facilitate the development and experimentation of collaborative AI agents. The project provides a modular framework that allows developers to define agents, environments, and interaction protocols, enabling complex simulations and research in distributed AI.

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/MAS_Project.git
cd MAS_Project

# Set up a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install required dependencies
pip install -r requirements.txt
```

## Usage

### Running a Sample Simulation

```bash
python -m mas_project.run --config examples/sample_config.yaml
```

The `--config` flag points to a YAML configuration file that defines the agents, their behaviors, and the environment settings.

### Importing the Library

```python
from mas_project.core import Agent, Environment

# Define a custom agent
class MyAgent(Agent):
    def step(self, observation):
        # Implement agent logic here
        return action

# Initialize environment
env = Environment(config_path='examples/sample_config.yaml')
env.add_agent(MyAgent())
env.run()
```

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Make your changes and ensure that all tests pass.
4. Commit your changes with clear commit messages.
5. Push your branch to your fork and open a pull request against the `main` branch.

Please adhere to the existing code style and include appropriate documentation and tests for new features.

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
