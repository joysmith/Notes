## Part 1

### Install python

1. install python 3.12.2 or above [click me](https://www.python.org/downloads/)

```py
python --version
```

<br>
<br>

### Docker installation and configuration

1. Install docker for window [click me](https://docs.docker.com/desktop/setup/install/windows-install/)

2. launch docker: Go to Volumes--> Create Volume--> Text box: "n8n_data" --> Create

3. In docker: Go to Images--> Search image to run--> "n8nio"--> pull

4. In docker: Go to Images--> **n8nio/n8n**--> run

   - Optional setting: Container name: n8n
   - Ports: 5678
   - click on run
   - Click on localhost link
   - Set up owner account
     - email: joysmith271@gmail.com
     - password: Jo123456789

-
-

5.

Note: Install WSL

### Ollama installation

1. Download and install Ollama locally [Click me](https://ollama.com/download)

```sh
irm https://ollama.com/install.ps1 | iex
```

2. In terminal run

```sh
ollama
```

3. Sign In, page will open. Sign In with google account


<br>

---

<br>

## Part 2

1. Go to n8n site and login with your account [n8n link](https://n8n.io/)
  - name: joy smith peter
  - password: Jo.........
  - user: joy7

2. Go to n8n the  select, + -->workflow --> personal 
<img src="assets/images/1.png" width="700">
3. Click on "Add first step" then in search: chat--> On new chat event
4. In Chat click on +, then in search: Agent--> AI agent
5. In "AI agent" click on "add chat model", then in search: Open AI---> 
    - In parameter window create new credentials
    - Go to ["Open AI credentials"](https://platform.openai.com) and get API key
    - copy and paste the API key to 
    - Model select--> gpt 4.0 mini
6. Open chat gpt and type prompt "create a table format data for 100 patient with different hypertension reading", then click on copy.
7. Go to google sperad sheet and paste data in it. or type [sheet.new](sheet.new)
8. In n8n, "AI agent" click on memory, then in search select "simple memory"
9. In n8n. "AI agent" click on tool, then in search: google --> google sheet tool
    - 