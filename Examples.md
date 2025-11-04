# Add GPG key
curl -s https://packages.wazuh.com/key/GPG-KEY-WAZUH | sudo gpg --dearmor -o /usr/share/keyrings/wazuh-keyring.gpg

# Add repository
echo "deb [signed-by=/usr/share/keyrings/wazuh-keyring.gpg] https://packages.wazuh.com/4.x/apt/ stable main" | sudo tee /etc/apt/sources.list.d/wazuh.list

# Update package list
sudo apt update

# Install agent version 4.14.0-1
sudo apt install wazuh-agent=4.14.0-1 -y
