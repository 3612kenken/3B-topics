

# **Group Activity: GitHub Version Control (HTML + JavaScript) by Sir Kenneth Omiping**

## **Group Setup**

-   **3 students per group**
    
    -   **Student A – HTML Developer**
        
    -   **Student B – JavaScript Developer**
        
    -   **Student C – Integrator / Team Leader**
        



## **Step 1 – GitHub Account (All Students)**

1.  Go to https://github.com
    
2.  Sign up and verify email
    
3.  Log in successfully
    



## **Step 2 – Create Repository (Student C)**

-   Repository name: `simple-html-js-project`
    
-   Public → Add `README.md`
    
-   Invite Student A & B as collaborators
    



## **Step 3 – Clone Repository (All Students)**

```bash
git clone https://github.com/USERNAME/simple-html-js-project.git
cd simple-html-js-project
```



## **Step 4 – Initial Files (Student C)**

### **index.html**

```html
<!DOCTYPE html>
<html>
<head>
    <title>GitHub Group Activity</title>
</head>
<body>
    <h1>Welcome</h1>
    <button onclick="showMessage()">Click Me</button>
    <p id="output"></p>

    <script src="script.js"></script>
</body>
</html>
```

### **script.js**

```javascript
function showMessage(){
    document.getElementById("output").innerText = "Hello from JavaScript!";
}
```

```bash
git add .
git commit -m "Initial HTML and JS setup"
git push origin main
```



## **Step 5 – Pull Latest Changes (Student A & B)**

```bash
git pull origin main
```



## **Step 6 – Create Branches**

### **Student A**

```bash
git checkout -b html-feature
```

### **Student B**

```bash
git checkout -b js-feature
```



## **Step 7 – Role-Based Coding Any HTML Codes You Want**

### **Student A – HTML - Sample**

```html
<h2>Group Members</h2>
<ul>
    <li>Student A</li>
    <li>Student B</li>
    <li>Student C</li>
</ul>

<button onclick="changeColor()">Change Background</button>
```

```bash
git add index.html
git commit -m "Added group members and button"
git push origin html-feature
```



### **Student B – JavaScript - Sample**

```javascript
function changeColor(){
    document.body.style.backgroundColor = "lightblue";
}
```

```bash
git add script.js
git commit -m "Added background color function"
git push origin js-feature
```



## **Step 8 – Merge (Student C)**

1.  Open **Pull Requests** on GitHub
    
2.  Merge `html-feature`
    
3.  Merge `js-feature`
    



## **Step 9 – Final Pull (All Students)**

```bash
git checkout main
git pull origin main
```

## **Expected Output**

-   HTML page with group list
    
-   Button changes background color
    
-   All students have commits in GitHub
    


## **Key Concepts Reinforced**

-   GitHub accounts
    
-   Clone, branch, commit, push, pull
    
-   Role-based collaboration




