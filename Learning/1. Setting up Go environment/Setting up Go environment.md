1. Download Go:
Visit the official Go website (https://golang.org) and navigate to the "Downloads" page. Choose the appropriate distribution for your operating system (Windows, macOS, or Linux) and download the installer.

2. Install Go:
Run the installer you downloaded and follow the installation instructions for your operating system. The installer will guide you through the process and set up Go on your machine.

3. Set up environment variables:
After installing Go, you need to set up environment variables to ensure that your system recognizes the Go installation. The steps for setting environment variables vary depending on your operating system:

* Windows:
Open the Control Panel and go to "System and Security" > "System" > "Advanced system settings".
In the System Properties window, click on the "Environment Variables" button.
In the "User variables" section, click "New" to add a new variable.
Set the variable name as "GOPATH" and the variable value as the path to your Go workspace directory. For example, C:\Users\YourUsername\go.
Edit the "Path" variable and append C:\Go\bin (or the directory where Go is installed) to the existing values.
Click "OK" to save the changes.

* macOS and Linux:
Open a terminal.
Open your shell profile file. For macOS, it's typically ~/.bash_profile, ~/.bashrc, or ~/.zshrc. For Linux, it's usually ~/.bashrc or ~/.bash_profile.
Add the following lines to the file, replacing /usr/local/go with the path where Go is installed:

```bash
export GOPATH=$HOME/go
export PATH=$PATH:/usr/local/go/bin:$GOPATH/bin
```
Save the file and exit the text editor.
Run source <profile_file> to apply the changes to your current session. For example, source ~/.bash_profile.

4. Verify the installation:
Open a new terminal or command prompt window and run the following command:

```bash
go version
```
If the installation was successful, it should display the installed Go version.

5. Create your Go workspace:
Go uses a workspace directory to organize your Go projects and packages. Create a directory to serve as your workspace, such as ~/go (for macOS and Linux) or C:\Users\YourUsername\go (for Windows).

6. Test your Go installation:
Create a new file named hello.go and open it in a text editor. Add the following code:
```Go
package main

import "fmt"

func main() {
    fmt.Println("Hello, Go!")
}

```
Save the file and navigate to the directory containing hello.go in your terminal or command prompt. Run the following command:
```Go
go run hello.go
```
If everything is set up correctly, it should output "Hello, Go!".

Congratulations! You have successfully set up your Go environment. You can now start writing and running Go programs on your machine.


