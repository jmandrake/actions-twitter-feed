# actions-twitter-feed

1. Get the weather forecast

2. To do: Send a tweet to my account with that info

## Resources:

Python automation ideas(https://www.youtube.com/watch?v=VLNcnROUTb8)



## How to update installation
sudo apt-get update

## Compile Python and Create VirtualEnv with it
sudo apt-get install build-essential gdb lcov libbz2-dev libffi-dev libgdbm-dev liblzma-dev libncurses5-dev libreadline6-dev libsqlite3-dev libssl-dev lzma lzma-dev tk-dev uuid-dev zlib1g-dev

### Download Python source tarball
wget https://www.python.org/ftp/python/3.11.1/Python-3.11.1.tgz

tar xzvf Python-3.11.1.tgz

rm Python-3.11.1.tgz

cd into Python-3.11.1

### Run the configuration script and creates the Makefile
./configure --enable-optimizations

### Compile Python and use both cpu cores as seen in htop
make -j 2

### Final step puts everything in place
sudo make altinstall


### Use the latest Python version
/usr/local/bin/python3.11

vim ~/.bashrc

add this alias:
alias python="/usr/local/bin/python3.11"

Remove the Python source dir from the project folder:
rm -rf Python-3.11.1

