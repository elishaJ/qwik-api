<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/221352995-5ac18bdf-1a19-4f99-bbb6-77559b220470.gif" alt="MasterHead">
</div>

<h1 align="center">Qwik API</h1>

This repository contains a collection of Flask API endpoints designed to simplify the usage and execution of tasks using the Cloudways API. These endpoints are designed to return filtered JSON data directly, eliminating the need for additional processing and filtering on the client side.

### Layout

```tree
├── apps
│   └── apps.py
├── auth
│   ├── create_keys.py
│   └── ssh_auth.py
├── cleanup
│   ├── cleanup.py
│   ├── delete_keys.py
│   └── key_info.py
├── servers
│   └── servers.py
├── token
│   └── auth_token.py
├── .gitignore
└── README.md

```

A brief description of the layout:

* `apps` folder for apps endpoint files.
* `apps.py` fetches app info filtered by project/server ID. 
* `auth` folder for auth endpoint files.
* `create_keys.py` stores key ID(s) created by `ssh_auth.py` to GCP Firestore.
* `ssh_auth.py` creates and uploads SSH key(s) to Cloudways server(s).
* `cleanup` folder for cleanup endpoint files. 
* `cleanup.py` deletes SSH key(s) from Cloudways server(s).
* `delete_keys.py`deletes key ID(s) from Firestore. 
* `key_info.py`fetches key ID(s) for deletion.
* `servers` folder for servers endpoint files.
* `servers.py` fetches server information based on different routes. See API reference for details.
* `token` folder for token endpoint files.
* `auth_token.py` script generates and returns authentication token.
* `.gitignore` file specifying which files and directories to ignore in version control.
* `README.md` Project README file providing an overview of the project and its components.


### Roadmap

- [x] Generate and filter authentication token.
- [x] Fetch IDs of all servers under account.
- [x] Fetch public IP of all servers under account.
- [x] Fetch SSH user names of running servers.
- [x] Fetch app info filtered by server ID.
- [x] Fetch app info filtered by project ID.
- [x] Set up SSH keys on all running servers.
- [x] Set up SSH keys on server(s) filtered by project ID.
- [x] Set up SSH keys on server(s) filtered by server ID.
- [x] Export key ID(s) to GCP Firestore
- [x] Create endpoint to remove keys from Cloudways server and Firestore.

### Built with

<a href="https://www.python.org/"><img src="https://user-images.githubusercontent.com/74038190/212257472-08e52665-c503-4bd9-aa20-f5a4dae769b5.gif" alt="Python Logo" width="40" height="40"></a> <a href="https://cloud.google.com/firestore/"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSiDj0DEGHE3SO6cpqBrV36WVBmLbIDPbtuzk3Xsf9jtg&s" alt="GCP Firestore" width="40" height="40"></a>



###  Skills
- Python development
- GCP Firestore database management

### Badges

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)


### Feedback

If you have any feedback, please reach out to me at elisha.jamil@gmail.com