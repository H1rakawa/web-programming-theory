---
title: Lập trình Web 🖥️
markmap:
  colorFreezeLevel: 2
  color:
      - "#4287f5"
      - "#34a853"
      - "#fbbc05"      
      - "#ea4335"
      - "#ff69B4"
---
# **Lập trình Web** 🖥️

## **1. Kiến thức cơ bản về lập trình web**
### **1.1. Tổng quan về Web**
#### **1.1.1. Web hoạt động như thế nào?**
##### **→ Khi bạn nhập URL vào trình duyệt, điều gì xảy ra?**
##### 1.1.1.1. Trình duyệt gửi yêu cầu HTTP đến server.
##### 1.1.1.2. Server xử lý và phản hồi HTML, CSS, JS.
##### 1.1.1.3. Trình duyệt tải và hiển thị nội dung web.
##### 1.1.1.4. Nếu có API, JavaScript sẽ gửi request đến API để lấy dữ liệu động.

### **1.2. HTTP & HTTPS**
#### **HTTP (HyperText Transfer Protocol) là giao thức giúp client và server giao tiếp với nhau.**
#### **HTTPS là phiên bản bảo mật của HTTP, sử dụng SSL/TLS để mã hóa dữ liệu.**

## **2. Frontend Development**
### **2.1. HTML (HyperText Markup Language)**
#### **2.1.1. Cấu trúc HTML cơ bản**
```html
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Đầu Tiên</title>
</head>
<body>
    <h1>Xin chào thế giới!</h1>
</body>
</html>
```

#### **2.1.2. Các thẻ quan trọng**
- **Thẻ tiêu đề:** `<h1> - <h6>`
- **Thẻ đoạn văn:** `<p>`
- **Thẻ danh sách:** `<ul>, <ol>, <li>`
- **Thẻ liên kết:** `<a href="link">`
- **Thẻ hình ảnh:** `<img src="image.jpg" alt="Mô tả">`
- **Thẻ form:** `<form>, <input>, <textarea>, <button>`

### **2.2. CSS (Cascading Style Sheets)**
#### **2.2.1. Cách viết CSS**
```css
/* CSS nội dòng */
<p style="color: red;">Đây là chữ màu đỏ</p>

/* CSS trong thẻ <style> */
<style>
    p { color: blue; }
</style>

/* CSS trong file riêng */
p { color: green; }
```

## **3. Backend Development**
### **3.1. Node.js & Express.js**
#### **3.1.1. Cài đặt Node.js**
```
npm init -y
npm install express
```

#### **3.1.2. Tạo server đơn giản**
```
const express = require("express");
const app = express();

app.get("/", (req, res) => {
    res.send("Xin chào từ server!");
});

app.listen(3000, () => console.log("Server chạy trên cổng 3000"));
```

## **4. DevOps & Triển khai**
### **4.1. Docker**
#### **4.1.1. Dockerfile**
```
FROM node:16
WORKDIR /app
COPY . .
RUN npm install
CMD ["node", "server.js"]
EXPOSE 3000
```

## **5. Công nghệ & các xu hướng**
### **5.1. Các công nghệ phổ biến**
#### **5.1.1. JavaScript Frameworks**
- **React.js:** Virtual DOM, component-based, state management với Redux/Zustand.
- **Vue.js:** Two-way binding, Vue Router, Vuex/Pinia.
- **Angular:** TypeScript, Dependency Injection, RxJS.

#### **5.1.2. Backend Frameworks**
- **Node.js (Express.js, NestJS)**
- **Python (Django, FastAPI)**
- **PHP (Laravel)**
- **Java (Spring Boot)**

#### **5.1.3. Database mới nổi**
- **NoSQL:** MongoDB, Firebase Firestore.
- **NewSQL:** CockroachDB, TiDB.
- **Graph Databases:** Neo4j.

### **5.2. Xu hướng & phát triển**
#### **5.2.1. JAMstack**
- Kiến trúc không máy chủ (Serverless), dùng API và CDN để tối ưu tốc độ.
- Frameworks phổ biến: Next.js, Nuxt.js.

#### **5.2.2. Web 3.0 & Blockchain**
- DApp (Decentralized Applications) sử dụng Ethereum, Solidity.
- Công nghệ IPFS (InterPlanetary File System) để lưu trữ phân tán.

#### **5.2.3. AI & Machine Learning trong Web**
- Chatbot thông minh (GPT, Watson AI).
- Cá nhân hóa nội dung bằng AI.

#### **5.2.4. Progressive Web Apps (PWA)**
- Ứng dụng web có trải nghiệm như app native.
- Công nghệ: Service Workers, Web App Manifest.

#### **5.2.5. Edge Computing & Serverless**
- AWS Lambda, Cloudflare Workers giúp xử lý dữ liệu gần người dùng hơn.
- Giảm tải cho backend truyền thống.