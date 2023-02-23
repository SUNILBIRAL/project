# project
GIT and GITHUB

What is a “version control system”? 
Version control systems are a category of software tools that helps in recording changes made to files by keeping a track of modifications done in the code.

Why Version Control system is so Important?
As we know that a software product is developed in collaboration by a group of developers they might be located at different locations and each one of them 
contributes to some specific kind of functionality/features. So in order to contribute to the product, they made modifications to the source code(either 
by adding or removing). A version control system is a kind of software that helps the developer team to efficiently communicate and manage(track)
all the changes that have been made to the source code along with the information like who made and what changes have been made. A separate branch is created
for every contributor who made the changes and the changes aren’t merged into the original source code unless all are analyzed as soon as the changes are green 
signaled they merged to the main source code. It not only keeps source code organized but also improves productivity by making the development process smooth.

What is Git Clone?
The git clone command is used to create a copy of a specific repository or branch within a repository. When you clone a repo you get a copy of the entire 
history of the repo. The command used for cloning any repository is:
git clone <repository-link>

HTTP vs SSH

SSH

SSH (Secure Shell) is a public-key cryptography protocol that ensures no one can intercept or change the data during the transfer. Since it is more difficult
to set up, it is not as widespread as HTTPS, but it offers greater data integrity and security.
However, firewalls on some systems refuse to allow SSH connections on the default port, which can further complicate the setup. Additionally, some operating systems 
don't have SSH clients installed by default.

Why Use SSH for Git?
The purpose of establishing an SSH connection is to encrypt data exchanged between the client and the server. SSH connections are based on a key pair - a private key 
on a remote server and thecorresponding public key on thelocal system.
Using SSH keys means there is no need to provide the username and password for each action, for example, pushing or pulling changes or signing commits.

HTTPS

HTTPS (Hyper Text Transfer Protocol Secure) is a more widespread network protocol that uses SSL/TLS data encryption. Since it is easier to configure than SSH, HTTPS
is more common but provides a lower data security level since it doesn't use public-key cryptography.

Git with HTTPS uses token-based authentication to establish connections on port 443 via the Public/Private Pair authentication mode. Port 443 is open in almost 
every firewall, which isn’t always the case for SSH.
The downside of using HTTPS is that every action, such as git fetch, git pull, or git push asks for your username and password.

Why Use HTTPS for Git?
The main purpose of HTTPS is to allow secure data transfers between the client and server. HTTPS facilitates Git setup as there is no need to create SSH keys 
for each machine from which you want to access the repository.
The authentication is performed through a Personal Access Token, which acts as a unique password and allows users to additionally secure their account with 2FA.

The benefits of using HTTPS for Git are:
Simple setup. HTTPS is easy to set up, requiring only the repo URL and the clone command.
Availability. HTTPS is available on every operating system and has very few firewall restrictions.
Portability. Access the repository from any machine by providing the username and password/token.

Local Repository and Remote Repository
Local repositories reside on the computers of team members. In contrast, remote repositories are hosted on a server that is accessible for all team members -
most likely on the internet or on a local network. Technically, a remote repository doesn't differ from a local one: it contains branches, commits, and tags 
just like a local repository.

About 90% of version control related work happens in the local repository: staging, committing, viewing the status or the log/history, etc. Moreover, 
if you're the only person working on your project, chances are you'll never need to set up a remote repository.
Only when it comes to sharing data with your teammates, a remote repo comes into play. Think of it like a "file server" that you use to exchange data with your colleagues.
Let's look at the few things that distinguish local and remote repositories from each other:
reffer this link----- https://www.git-tower.com/learn/git/ebook/en/command-line/remote-repositories/introduction/#:~:text=Local%20repositories%20reside%20on%20the%20computers%20of%20team,commits%2C%20and%20tags%20just%20like%20a%20local%20repository.
