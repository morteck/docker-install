Docker Install Script

A simple shell script to install Docker Engine and related plugins on a Debian-based Linux distribution.
This script automates adding Docker’s GPG key, configuring the repository, installing the necessary packages, and running a test container.

---

📜 Features

Automatically adds Docker's official GPG key and repository.

Installs:

docker-ce

docker-ce-cli

containerd.io

docker-buildx-plugin

docker-compose-plugin


Verifies installation by running the hello-world container.

Minimal interaction required.



---

🚀 Usage

1. Clone this repository
```
git clone https://github.com/morteck/docker-install.git
cd docker-install
```
2. Make the script executable
```
chmod +x install_docker.sh
```
3. Run the script
```
./install_docker.sh
```
The script will:

1. Update system packages


2. Add Docker’s GPG key and repository


3. Install Docker and plugins


4. Run a quick test container


5. Print Done! when finished




---

🛠️ Requirements

Debian or Debian-based distribution (Ubuntu, Pop!_OS, Linux Mint, etc.)

apt-get package manager

sudo privileges

Internet access for downloading packages



---

🔍 Example Output

When installation completes successfully, you should see Docker's Hello from Docker! message:
```
Hello from Docker!
This message shows that your installation appears to be working correctly.
```

---

📄 License

This project is licensed under the Apache License 2.0. See the LICENSE file for full details.


---

💡 Notes

This script is intended for clean installations.

If Docker is already installed, you may want to remove old versions first:
```
sudo apt-get remove docker docker-engine docker.io containerd runc
```
Customize the script as needed for your environment.

---

© 2025 Mikael Todd. Created and maintained by [Mikael Todd](https://github.com/morteck). 
