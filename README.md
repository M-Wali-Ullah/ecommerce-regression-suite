# 🛍️ E-Commerce API Regression Suite

This project is an **Automated Regression Suite** for E-Commerce APIs, built using **Postman** and **Newman**. It allows automated testing of core API flows such as user registration, login, product browsing, cart management, and order retrieval.  

The suite is also integrated with **GitHub Actions** for CI/CD automation, generating **HTML test reports** after every push or pull request.

---

## 🚀 Features

- ✅ User registration and login tests  
- ✅ Product listing and details verification  
- ✅ Cart creation and retrieval  
- ✅ Order-related endpoints testing  
- ✅ Automated HTML report generation using Newman + htmlextra  
- ✅ CI/CD integration with GitHub Actions  

---

## 📦 Project Setup

### 1. Clone the repository
```bash
git clone https://github.com/M-Wali-Ullah/ecommerce-api-regression-suite.git
cd ecommerce-regression-suite
```

### 2. Install dependencies
```bash
npm install
```

### 3. Folder structure
```
ecommerce-api-regression-suite/
 ┣━ postman/
 ┃   ┣━ ecommerce_collection.json        # Postman collection
 ┃   ┗━ staging_environment.json         # Postman environment
 ┣━ reports/                             # Generated HTML reports
 ┣━ package.json
 ┣━ package-lock.json
 ┗━ .github/
     ┗━ workflows/
         ┗━ api-tests.yml                # GitHub Actions workflow
```

## 🧪 Run Tests Locally

You can run the Postman collection locally using **npm scripts**:

```bash
npm test
```

- Reports will be generated at `reports/ecommerce-report.html`  
- Open the HTML file in a browser to view detailed test results

---

## ⚙️ GitHub Actions CI/CD

The workflow is defined in `.github/workflows/api-tests.yml` and automatically:

1. Installs Node.js and dependencies  
2. Ensures `reports/` folder exists  
3. Runs Newman tests with HTML report generation  
4. Uploads `ecommerce-report.html` as an artifact  

The workflow triggers on:

- `push` to `main`  
- Pull requests targeting `main`

---

## 🔧 Environment Variables

The Postman environment `staging_environment.json` contains:

| Variable | Description |
|----------|-------------|
| `baseUrl` | Base URL of the API (`https://fakestoreapi.com`) |
| `token`   | Stores auth token after login |
| `userId`  | Stores user ID after registration/login |
| `productId` | Stores product ID for cart operations |

---

## 📄 Report Generation

- HTML reports are generated automatically via **Newman + htmlextra**  
- In GitHub Actions, reports are uploaded as **artifacts** and can be downloaded for review

---

## 💻 References

- [Postman](https://www.postman.com/)  
- [Newman](https://www.npmjs.com/package/newman)  
- [Newman HTML Extra Reporter](https://www.npmjs.com/package/newman-reporter-htmlextra)  
- [Fake Store API](https://fakestoreapi.com/)

