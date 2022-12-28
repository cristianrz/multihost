# multihost

multihost is a script that runs a given script on multiple hosts specified in a
host file via ssh.

## Install

```
git clone https://github.com/cristianrz/multihost.git
cd multihost
make
make install
```

## Usage

```
./multihost [-i host_file] [-v] script_file
```

## Options

- `-i host_file`: Specify a host file other than the default hosts.txt.
- `-v`: Enable verbose output.

## Arguments

- `script_file`: The script file to be run on each host.

## Example

To run the script myscript.sh on the hosts specified in myhosts.txt:

```
./multihost -i myhosts.txt myscript.sh
```
