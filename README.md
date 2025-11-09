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

## 📦 Project ScreenShots

<img width="1861" height="828" alt="image" src="https://github.com/user-attachments/assets/0b5b380a-10a1-4c32-a89c-1b15f6a74bcf" />
<img width="1919" height="973" alt="image" src="https://github.com/user-attachments/assets/6cad7278-7b7d-47fd-a618-25a6c796c95c" />
<img width="1918" height="962" alt="image" src="https://github.com/user-attachments/assets/34080dcc-fc46-48e8-81df-858668ccc24a" />
<img width="1912" height="961" alt="image" src="https://github.com/user-attachments/assets/cb85a3e8-3e65-4eb1-a65b-e97f9405cc8b" />
<img width="1919" height="972" alt="image" src="https://github.com/user-attachments/assets/f041c87e-837f-48ab-ac37-4560b43d62c6" />

---

## 📄 Report Generation

- HTML reports are generated automatically via **Newman + htmlextra**  
- In GitHub Actions, reports are uploaded as **artifacts** and can be downloaded for review
<img width="1145" height="748" alt="image" src="https://github.com/user-attachments/assets/24387ba4-433e-42fa-b9a5-6079d21af92a" />
<img width="1101" height="514" alt="image" src="https://github.com/user-attachments/assets/7d8c3d7e-ca39-4dbe-b615-1c86d9139611" />

---

## 📦 Project Folder structure
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
## 💻 References

- [Postman](https://www.postman.com/)  
- [Newman](https://www.npmjs.com/package/newman)  
- [Newman HTML Extra Reporter](https://www.npmjs.com/package/newman-reporter-htmlextra)  
- [Fake Store API](https://fakestoreapi.com/)

