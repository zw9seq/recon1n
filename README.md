# Recon1n

> A comprehensive tool for performing various types of scans on a target.

**Recon1n** is a **Bash script** that consolidates multiple commonly used reconnaissance tools into a single suite, enabling you to perform thorough target reconnaissance more efficiently. It was designed to save time when gathering information on a target, which can range from individual hosts to multiple hosts and even entire networks. 

The script is structured into two main phases: **anonymization**, where you can change your MAC address and route your traffic through the TOR network for anonymity; and **reconnaissance**, where you can execute multiple scans over different services to gather valuable information.

This tool is ideal for identifying potential vulnerabilities and attack vectors in a target system or network.

## Installation

### Clone the Repository

Start by cloning the repository to your preferred directory:

```bash
git clone https://github.com/zw9seq/recon1n
cd recon1n
```

### Install Dependencies

Next, install the required dependencies using the **setup.sh** script:

```bash
./setup.sh
```

Once the necessary packages are installed, you will need to configure the script to work properly.

### Configuration

Open the script with your preferred text editor. For example:

```bash
nano recon1n
```

Then, modify the following lines:

```bash
small_list=""
medium_list=""
big_list=""
```

You need to specify the paths to your desired wordlists for subdirectory fuzzing. A comprehensive set of wordlists can be found here: [https://github.com/danielmiessler/SecLists].

### Optional Configuration: Adding to System PATH

For easier execution, you can add the script to your system's PATH. To check your current PATH, run:

```bash
echo $PATH
```

Typically, you'll want to place the script in the **/usr/local/bin** directory. To do this, run:

```bash
sudo cp recon1n /usr/local/bin
```

This allows you to run the script from anywhere on your system without needing to navigate to the script's directory.

## Usage

To run **Recon1n**, simply execute the following command:

```bash
./reconin
```

This will present a menu with all available options in the script. You can select an option by typing the corresponding number.

Within the reconnaissance functions, some options will prompt you for additional input or display a secondary menu for further choices. You may also be asked to provide specific information needed for the tool to perform the scans.

## License

This project is licensed under the **MIT License**. Feel free to modify and distribute it as needed.

See the [LICENSE](LICENSE) file for more details.
