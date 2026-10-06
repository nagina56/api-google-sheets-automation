# 🔄 API to Google Sheets Automation

An automation workflow built with **n8n** that fetches data from a public REST API and automatically adds the retrieved data to Google Sheets.

This project demonstrates how APIs and workflow automation can be combined to collect and organize data without manually entering it into a spreadsheet.

## ✨ Features

* Fetches data from a public REST API
* Uses an HTTP GET request
* Processes JSON API responses
* Splits API data into individual records
* Automatically adds data to Google Sheets
* Uses n8n for workflow automation
* Reduces manual data entry

## 🛠️ Technologies Used

* **n8n**
* **REST API**
* **HTTP Request**
* **Google Sheets**
* **JSON**
* **Workflow Automation**

## 🌐 API Used

This project uses the free **JSONPlaceholder API** for testing and learning.

API endpoint:

```text
https://jsonplaceholder.typicode.com/users
```

No API key is required.

## 🔄 Workflow

The automation follows this workflow:

```text
Manual Trigger
      ↓
HTTP Request
      ↓
Split Out
      ↓
Google Sheets
```

### How It Works

1. **Manual Trigger** starts the workflow.
2. **HTTP Request** sends a GET request to the public API.
3. The API returns user data in JSON format.
4. **Split Out** processes individual user records.
5. **Google Sheets** adds each record to a new row automatically.

## 📸 Workflow Screenshot

The n8n workflow:

![n8n Workflow](screenshots/n8n-workflow.png)

## 📊 Google Sheets Output

The fetched API data is automatically added to Google Sheets.

![Google Sheets Output](screenshots/google-sheet-output.png)

## 📋 Example Data

The API returns information such as:

| ID | Name             | Username  | Email                                           |
| -- | ---------------- | --------- | ----------------------------------------------- |
| 1  | Leanne Graham    | Bret      | [Sincere@april.biz](mailto:Sincere@april.biz)   |
| 2  | Ervin Howell     | Antonette | [Shanna@melissa.tv](mailto:Shanna@melissa.tv)   |
| 3  | Clementine Bauch | Samantha  | [Nathan@yesenia.net](mailto:Nathan@yesenia.net) |

## ⚙️ Setup

### 1. Install n8n

This project was created using a local n8

