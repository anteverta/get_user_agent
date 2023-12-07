# Get User Agent

`get_user_agent` is a simple Python library to generate random user agents based on different criteria such as browser, operating system, and device type. It provides an easy way to retrieve user agents for testing and other purposes.

## Installation

To use `get_user_agent`, you can install it using `pip`. Open a terminal and run:

```bash
pip install get_user_agent
```
## Usage
```
from get_user_agent import GetUserAgent

# Create an instance of the GetUserAgent class
user_agent_gen = GetUserAgent()

# Get a random user agent for a specific browser, OS, and device type
random_agent = user_agent_gen.random(browser='Chrome', os='Windows', device='desktop')
print("Random User Agent (filtered):", random_agent)

# Get a random user agent for a specific browser
random_browser_agent = user_agent_gen.by_browser(browser='Firefox')
print("Random User Agent by Browser:", random_browser_agent)

# Get a random user agent for a specific operating system
random_os_agent = user_agent_gen.by_os(os='iOS')
print("Random User Agent by OS:", random_os_agent)

# Get a random user agent for a specific device type
random_device_agent = user_agent_gen.by_device(device='mobile')
print("Random User Agent by Device:", random_device_agent)

# Get a list of user agents for a specific browser
browser_agents = user_agent_gen.list_by_browser(browser='Chrome')
print("User Agents by Browser:", browser_agents)

# Get a list of user agents for a specific operating system
os_agents = user_agent_gen.list_by_os(os='Android')
print("User Agents by OS:", os_agents)

# Get a list of user agents for a specific device type
device_agents = user_agent_gen.list_by_device(device='tablet')

print("User Agents by Device:", device_agents)

# Get a list of all user agents
all_agents = user_agent_gen.list_all()
print("All User Agents:", all_agents)
```
