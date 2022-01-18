# Selenium Grid with Appium using Ansible (OSX)

# Installation
## Prerequisites: You will require at minimum Java 8, Python 2.7 and Xcode already installed

# Install dependencies
      brew install ansible screen

# Start and register the grid
      ansible-playbook setup.yaml -i inventory.ini

# Selenium Grid Web GUI 
      localhost:4444/grid/console

      This port can be changed, by changing the value of 'selenium_hub_port' in the 'main.yaml' file.

# Default Nodes 
      Mobile Safari Testing on:
      - iPhone 11 
      - iPhone 12

      Mobile App Testing on:
      - iPhone 11 Pro
      - iPhone 12 Pro

# Configuring Nodes
      Add or remove devices in 'configure_browser_nodes.yaml' or 'config_app_nodes.yaml'.

      You may also need to add/remove ports accordingly inside 'start_appium_nodes.yaml'.

# Selenium Grid Server Files
      Downloaded to the 'Users/shared/server' directory.

      Configurable inside 'main.yaml'.
