# 📌 API Testing with Postman

## 📖 Overview

This repository contains **API test collections and environments** created using **Postman**.
It is designed to demonstrate API automation, environment setup, and integration with CI/CD pipelines.

---

## 🗂️ Repository Structure

```
API-Testing-Postman/
│── collection.json        # Postman collection with API requests
│── environment.json       # Postman environment file
│── reports/               # Test execution reports (e.g., Newman HTML reports)
│── README.md              # Project documentation
```

---

## 🚀 Getting Started

### 1️⃣ Prerequisites

* Install [Postman](https://www.postman.com/downloads/)
* Install [Node.js](https://nodejs.org/) (for Newman CLI runner)
* Install [Newman](https://www.npmjs.com/package/newman)

```bash
npm install -g newman
```

### 2️⃣ Run Collection via Newman

Run collection with environment file:

```bash
newman run collection.json -e environment.json
```

Run collection with HTML report:

```bash
newman run collection.json -e environment.json -r cli,html
```

Reports will be saved in the `reports/` folder.

---

## 📊 Example Use Cases

✔️ Validate REST API endpoints
✔️ Check response codes & response time
✔️ Verify authentication & error handling
✔️ Automate API regression tests

---

## 🔗 CI/CD Integration (Future Scope)

* Run Newman in **GitHub Actions**
* Publish reports automatically
* Integrate with tools like **Jenkins / GitLab CI**

---

## 👩‍💻 Author

* Krishna Yadav 
* ✉️ Contact: \er.krishnayd@gmail.com
* 🌐 LinkedIn/GitHub: \[links]


---

Do you want me to also **add GitHub Actions workflow file (`.yml`)** so your repo can **automatically run Postman tests** on every push?
