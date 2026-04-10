# chatbot
AI pract


Step 1 — Check if Python is installed<br>
Open your Ubuntu terminal and run:<br>
bashpython3 --version<br>
You should see something like Python 3.10.x. Python 3 comes pre-installed on most Ubuntu versions, so you're likely good.<br><br>

Step 2 — Install pip (Python package manager)<br>
bashsudo apt update<br>
sudo apt install python3-pip -y<br>
Verify it works:<br>
bashpip3 --version<br><br>

Step 3 — Install Flask<br>
bashpip3 install flask<br><br>

Step 4 — Create the project folder<br>
bashmkdir college_chatbot<br>
cd college_chatbot<br>
mkdir templates<br><br>

Step 5 — Create the files<br>
Use the nano text editor (built into Ubuntu) to create each file.<br>
Create bot.py:<br>
bashnano bot.py<br>
Paste the bot.py code from earlier, then press Ctrl+O to save and Ctrl+X to exit.<br>
Create app.py:<br>
bashnano app.py<br>
Paste the app.py code, then Ctrl+O → Ctrl+X.<br>
Create the HTML file:<br>
bashnano templates/index.html<br>
Paste the index.html code, then Ctrl+O → Ctrl+X.<br><br>

Step 6 — Run the app<br>
bashpython3 app.py<br>
You'll see:<br>
 * Running on http://127.0.0.1:5000<br><br>

Step 7 — Open in browser<br>
If you're on Ubuntu with a desktop (GUI), open Firefox or Chrome and go to:<br>
http://127.0.0.1:5000<br>
Your chatbot will be live!<br><br>

If you're on Ubuntu Server (no GUI)
If it's a remote server without a browser, you can make Flask accessible from another device on the same network. Change the last line of app.py:
python# Change this:
app.run(debug=True)

# To this:
app.run(host="0.0.0.0", port=5000, debug=True)
Then find your server's IP address:
bashhostname -I
Now open a browser on any device on the same network and go to:
http://<your-server-ip>:5000




to run:
cd college_chatbot<br>
python app.py

http://172.16.3.204:5000
