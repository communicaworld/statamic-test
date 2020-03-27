# Statamic + Vagrant

## Preparing the Environment

- **Install VirtualBox**: [Follow the instructions here](https://www.virtualbox.org/wiki/Downloads) to install VirtualBox on your particular operating system.

- **Install Vagrant**: [Follow the instructions here](https://www.vagrantup.com/downloads.html) to install Vagrant on your particular operating system.

## Configuration

- **Your .env File**: Copy the `config/vagrant/.env.example` file to a new `.env` file in the same directory. 

- **(Optional) GitHub Authentication Token**: Alter the `GITHUB_AUTH_TOKEN` variable to your personal Github Authentication Token. [Follow the instructions here](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line) to setup your Github Authentication Token. This will help speed up the provisioning process.

- **(Optional) Statamic Credentials**: Alter the `STATAMIC_ADMIN_EMAIL` and `STATAMIC_ADMIN_PASS` variables to to your preferred access credentials.

## Vagrant Up

- **Run Vagrant Up**: Run `vagrant up` to provision the vagrant instance.

- **.www**: A `.www` folder will be created during the provisioning. This is where Statamic files can be altered. `.www/public` is your Apache DocumentRoot.

- **localhost:8001**: Navigate in your browser to `http://localhost:8001/` to view your Statamic website. You may log into your control panel at `http://localhost:8001/cp/auth/login` using the credentials specified in your `.env` file.

