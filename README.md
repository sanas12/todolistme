# ToDoListMe Automation Project

## 📌 Project Overview

This project automates task management on [ToDoListMe](https://todolistme.net/) using **Selenium WebDriver** with **C#** and **NUnit**. It performs the following operations:

- Adding multiple tasks from a JSON file
- Adding a single task
- Marking tasks as done
- Taking screenshots upon success or failure
- Logging test execution using **Extent Reports**

## 🛠️ Tech Stack

- **Programming Language:** C#
- **Frameworks:** NUnit, Selenium WebDriver
- **Reporting:** ExtentReports
- **Data Handling:** JSON
- **Test Execution:** NUnit Test Runner

## 📂 Project Structure

```
📦 todolistme
 ┣ 📂 BaseClass
 ┃ ┗ 📜 BaseTest.cs        # Handles test setup & teardown
 ┣ 📂 Pages
 ┃ ┣ 📜 AddNewTask.cs      # Page Object Model for adding tasks
 ┃ ┣ 📜 TaskActions.cs     # Page Object Model for marking tasks as done
 ┣ 📂 TestScripts
 ┃ ┗ 📜 Module1.cs         # NUnit test cases for adding & marking tasks
 ┣ 📂 DataDrivenTesting
 ┃ ┗ 📜 DataDrivenTesting.cs # Handles JSON data loading
 ┣ 📂 Screenshot
 ┣ 📜 README.md            # Project documentation
```

## 🚀 Setup & Installation

### 1️⃣ Prerequisites

Ensure you have the following installed:

- .NET SDK (=8.0)
- NUnit Test Adapter
- Chrome WebDriver 
- Visual Studio (recommended)

### 2️⃣ Clone the Repository

```sh
git clone https://github.com/yourusername/todolistme-automation.git
cd todolistme-automation
```

### 3️⃣ Install Dependencies

```sh
dotnet restore
```

### 4️⃣ Update WebDriver Path

Ensure the WebDriver path is set correctly in `BaseTest.cs`.

## 🏃 Running the Tests

To execute tests, run:

```sh
dotnet test
```

Alternatively, use **Visual Studio**:

- Open Test Explorer (`Test` → `Test Explorer`)
- Click **Run All**

## 📝 Test Cases

### ✅ Add Multiple Tasks

- Loads tasks from `tasks.json`
- Adds them to the To-Do list
- Verifies task presence

### ✅ Add and Mark a Single Task as Done

- Loads a single task from `tasks.json`
- Adds the task
- Marks it as done
- Verifies task completion

## 📸 Screenshots & Reporting

- Screenshots are captured on success or failure (`Screenshot` folder)
- ExtentReports logs are available for each test run

## 🛠️ Customization

- Modify `tasks.json` to add your own tasks
- Update `WebDriverWait` timeouts if needed

## 🤝 Contributions

Contributions are welcome! Feel free to open an **issue** or **pull request**.

## 📄 License

MIT License. See `LICENSE` for details.

---

**Author:** Sowmya Sanala\
**GitHub:** [yourusername](https://github.com/sanas12)

