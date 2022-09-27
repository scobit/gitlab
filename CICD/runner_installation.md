## Install GitLab Runner on linux

#### official doc
https://docs.gitlab.com/runner/install/linux-repository.html

#### Add the official GitLab repository:
`curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash`

#### Install the latest version of GitLab Runner
`sudo apt-get install gitlab-runner`

#### check version
`sudo gitlab-runner --version`

#### check status
`sudo gitlab-runner status`

#### register runner
`sudo gitlab-runner register`

#### then type URL and registration token from Setting - CI/CD - Runners
#### enter description and tags (macos, local) and note
#### and executor type (shell)

#### start runner
sudo gitlab-runner start

#### configuration file
/etc/gitlab-runner/config.toml

## install npm on runner
#### install nodejs
`sudo apt install nodejs`
#### check version of nodejs
`node -v`
#### install npm
`sudo apt install npm`
#### check version of npm
npm -v

## Docker runner on linux
#### We nedd to install docker only, instead of having to install all the tools.
#### install docker
`sudo apt install docker.io`
#### add current user to docker group
`sudo usermod -aG docker $USER`
#### logout / login
#### check containers
`sudo docker ps`


# choose docker executor and the default docker image (alpine:3.15.1)
sudo gitlab-runner register

# start runner
sudo gitlab-runner start

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

