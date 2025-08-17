# GitHub Actions 🚀

GitHub Actions is a **built-in CI/CD tool** inside GitHub.  
It helps you **automate tasks** like testing, building, and deploying projects — basically, your **virtual assistant for development**.

---

## 🔑 Key Concepts

- **Workflow** → Automated process triggered by events.  
- **Event** → The thing that starts the workflow (e.g., push, pull request).  
- **Job** → A set of steps executed on a runner.  
- **Step** → Individual tasks in a job (like running a script).  
- **Runner** → The virtual machine that runs your jobs.

---

## ⚙️ Workflow Execution Flow

1. **Event occurs** → Workflow starts.  
2. **Jobs execute in parallel** (by default).  
3. Each job runs steps inside a runner.  

---

## 🎯 Why Use GitHub Actions?

✅ Automates builds & tests  
✅ Improves code quality  
✅ Auto-deployment  
✅ Scalable & Secure  

---

## 📂 Workflow Example

Below is a sample workflow YAML file.  
It triggers **on push to the `main` branch** and runs a job that prints a greeting.

```yaml
name: sagar regmi

on:
  push:
    branches: [ main ]

jobs:
  demo:
    runs-on: ubuntu-latest
    
    steps:
      - name: Greetings
        run: echo "hello sagar i am from vm"
