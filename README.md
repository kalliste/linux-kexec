# linux-kexec

This script provides an easy way for users to switch between installed Linux kernels using `kexec`, allowing a kernel to be loaded without a full system reboot.

## Features

- **Dynamic Initrd Discovery**: Automatically finds the initrd or initramfs for a given kernel.
- **POSIX Compliance**: Uses POSIX-compliant syntax for broad compatibility.
- **Kexec Execution**: Prepares and executes the `kexec` command.
- **Tool Check**: Verifies if `kexec` is installed, and provides installation commands if not.
- **Root Check**: Ensures the script is run with root privileges.
- **Kernel Listing**: Lists all available kernels, excluding rescue entries.
- **Current Kernel Display**: Shows the currently running kernel.
- **User Input**: Prompts the user to select from available kernels or confirm the only available kernel.
- **Automation**: Use `--latest` to boot to the latest installed kernel automaticly.

## Usage

1. **Ensure `kexec` is Installed**: The script will prompt you to install `kexec-tools` if it is not found.

2. **Run as Root or Sudo**: `kexec` requires root privileges, so the script must be run as root or sudo.

3. **Choose a Kernel**: When prompted, enter the number corresponding to the kernel version you wish to boot into.

4. **Check**: If there is only one kernel installed, you'll be asked to confirm if you want to boot into it.
