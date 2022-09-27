#### install gitlab runner on linux doc
https://docs.gitlab.com/runner/install/linux-repository.html

# Add the official GitLab repository:
curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash

# Install the latest version of GitLab Runner
sudo apt-get install gitlab-runner

# check version
sudo gitlab-runner --version

# check status
sudo gitlab-runner status

# register runner
sudo gitlab-runner register

# then type URL and registration token from Setting - CI/CD - Runners
# enter description and tags (macos, local) and note
# and executor type (shell)

# start runner
sudo gitlab-runner start

# configuration file
/etc/gitlab-runner/config.toml

# install npm on runner
sudo apt update
sudo apt install nodejs
node -v
sudo apt install npm
npm -v


### install gitlab runner on mac os doc
https://docs.gitlab.com/runner/install/osx.html

# Install GitLab Runner
brew install gitlab-runner

# Install GitLab Runner as a service and start it
brew services start gitlab-runner

# check version
gitlab-runner -version

# check status
brew services info gitlab-runner

# register runner
gitlab-runner register


### install gitlab runner on windows doc
https://docs.gitlab.com/runner/install/windows.html

# Create a folder somewhere in your system, ex.: C:\GitLab-Runner

# Download the binary for 64-bit or 32-bit and put it into the folder you created.

# rename file to
gitlab-runner

# run cmd as a administrator

# go to gitlab folder
C:\GitLab-Runner

# install
.\gitlab-runner install

# start
.\gitlab-runner start

# status
.\gitlab-runner status

# register runner with our GitLab instance
.\gitlab-runner register

