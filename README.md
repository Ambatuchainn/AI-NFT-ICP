# how to make dfx project:
# Install dfx with this command:
sh -ci "$(curl -fsSL https://internetcomputer.org/install.sh)"
#But before you install dfx in your system you need to have wsl(Windows Subsystme for Linux) for windows only this is the link:
https://learn.microsoft.com/en-us/windows/wsl/install
# make sure you have dfx in your system:
dfx --version
# here's how you make your dfx first project:
dfx new <your-projectname>
cd <your-projectname>
# Starts the replica, running in the background
dfx start --background
# Deploys your canisters to the replica and generates your candid interface
dfx deploy
# to stop the deploy:
lsof -i :<your_local_port>
kill [PID]
