# CYBR506-Docker
Docker lab
In order to run this lab (all in powershell):

# For freeradius docker implementation
Go into the directory of "./Freeradius/"
Execute "docker build -t lab6 ."
Execute "docker run -d --name <any_name_here> -p 1812:1812/udp -p 1813:1813/udp lab6:latest"

# For Flaskapp docker implementation
Go into the directory of "./flaskapp/"
Execute "docker build . -t flaskapp"
Execute "docker run -d --name <any_name_here> -p 5000:5000/tcp flaskapp"

# From website to test implementation
Go to: "172.17.0.1:5000" on your web browser while both freeradius and Flaskapp is running
Type in <yourusername> and <yourpassword> for username and password
Success!
