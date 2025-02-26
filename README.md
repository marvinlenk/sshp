# sshp
A nice and easy bash script to handle multiple port forwardings and ssh via a login node to a final host. Note: tailored to the uni bonn physics department.

# How to install
1. Make sure the script is located in a place listed in `$PATH`. If not, either append `$PATH` in your dotfiles (`.bashrc` or similar) or create a symlink (`ln -s`) in the `bin/` folder of your choice.

2. Make the script executable with `chmod +x sshp`.

# How to use
Output of `sshp -h`:
```
Usage: sshp [-d] [-p PORT] [-r PORT_RANGE] [-m HOST] [-u USERNAME] [-s]
  -d              Direct connection (without jump host)
  -p PORT         Port forwarding. Forward a single port.
  -r PORT_RANGE   Port range for port forwarding. Specify ports as XXXX-YYYY.
  -t HOST         Hostname 'target' to connect to, default:desktop12.physik.uni-bonn.de
  -n HOST         Hostname 'login node' to tunnel through, default:desktop12.physik.uni-bonn.de
  -u USERNAME     Username for SSH connection (default: current user)
  -s              Disable password authentication
  --help          Display this help message
Script location: somepath/sshp
```
