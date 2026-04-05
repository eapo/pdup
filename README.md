A little Bash script that you can use to upload files to https://pixeldrain.com/ from the terminal. This is very useful for showing log files to developers or making quick backups of remote files through SSH.

## Installation
1. To install it you can execute this command:

```bash
sudo wget https://raw.githubusercontent.com/eapo/pdup/master/pdup -O "/usr/local/bin/pdup"; sudo chmod +x "/usr/local/bin/pdup"
```

Or in [Android Termux](https://termux.dev/):

```bash
sudo wget https://raw.githubusercontent.com/eapo/pdup/master/pdup -O ~/pdup; sudo chmod +x ~/pdup
```

Explanation: The `wget` command downloads the script from _github_ and saves it to `/usr/local/bin/pdup` or `~/pdup` in _Termux_ so you can run it from the terminal. Then `chmod` makes it executable.

2. Generate a new [Pixeldrain API key](https://pixeldrain.com/api)
3. Edit the `pdup` file to paste the API key between `"` at this line: `API=""`

```bash
sudo nano "/usr/local/bin/pdup"
```

Or in [Android Termux](https://termux.dev/):

```bash
nano ~/pdup
```

## Usage
Then you can upload files from anywhere in the system using

```bash
pdup file.txt
```

