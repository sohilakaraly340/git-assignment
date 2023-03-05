# Assignment #1

Assuming two developers are called `dev1` and `dev2`

Kickoff the work:
1. `Dev1` forks this repository.
2. `Dev1` invites `Dev2` to collaborate with them on the project (settings -> collaborators -> Add people).
3. `Dev2` accepts the invitation found in their inbox.
4. `Dev1` adds a protection on master branch “Require a pull request before merging.”

Each change is a branch, and each branch requires a pull request to review.  
<br/>
### Create the homepage
<details>
  <summary>
    Dev1 creates a branch called “basic-homepage-ui” and adds this html code.
  </summary>
   
   ```html
   <html>
    <head>
        <!-- Add link here -->
    </head>
    <body>
        <!-- Insert navbar here -->

        <!-- Actual body -->
        <div style="margin: 5px">
            <h1>Git & GitHub assignment #2</h1>
            <p>This assignment is intended to help you understand Git by practice.</p>
            <!-- Insert paragraph here -->
            <a href="about.html">Click me</a>
        </div>
    </body>
  </html>
   ```
  
</details>  


<details>
  <summary>
    Dev2 creates a branch called "homepage-navbar" and creates a navbar using the following html code. 
  </summary>
   
   ```html
   <ul>
      <li><a href="#home" class="active">Home</a></li>
      <li><a href="#news">News</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><a href="#about">About</a></li>
   </ul>
   ```
  
</details>


<details>
  <summary>
    Dev1 creates styles.css file in branch "homepage-navbar" and adds the following styles. 
  </summary>
   
   ```css
   ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    background-color: #333;
  }
  
  li {
    float: left;
  }
  
  li a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
  }
  
  /* Change the color of the active link */
  .active {
    background-color: #4CAF50;
  }

  body {
    margin: 0;
  }
   ```
  
</details>


<details>
  <summary>
    Div2 links the styles.css file in the index.html using link tag in the header
  </summary>
  
  ```css
  <link rel="stylesheet" type="text/css" href="styles.css"/>
  ```
  
</details>


<details>
  <summary>
    Div1 creates a branch called "homepage-git-info" and adds the following paragraph describing git as a version control system (read it)
  </summary>
  
  ```html
  <p>
Git is a distributed version control system that has become the de facto standard for software development teams around the world.<br>It allows multiple developers to collaborate on a codebase, track changes, and revert to previous versions if needed.<br>Git is flexible and can be used for projects of any size, from small personal projects to large, complex software applications.<br>It is also highly customizable and has a vast ecosystem of tools and plugins available to help streamline development workflows. With Git, developers can work more efficiently and effectively, ensuring that their projects are always in a state of continuous improvement.
  </p>
  ```
  
</details><br>

Don't forget to create a branch for each feature.<br>

### Create the about page
<details>
  <summary>
    Div2 creates about.html page and adds the following html
  </summary>
  
  ```html
  <!DOCTYPE html>
<html>

<head>
    <title>About Us</title>
    <!-- Add style link here -->
</head>

<body>
    <h1>About Us</h1>
    <p>Welcome to our website! We are a company that specializes in selling high-quality products for a variety of
        needs. Our goal is to provide our customers with the best possible experience when shopping with us.</p>

    <h2>Our Team</h2>
    <p>Our team consists of experienced professionals who are dedicated to providing exceptional customer service. We
        work hard to ensure that our customers are satisfied with their purchases and that their needs are met.</p>

    <h2>Our Products</h2>
    <p>We offer a wide range of products to meet the needs of our customers. Whether you're looking for electronics,
        home goods, or outdoor equipment, we've got you covered. All of our products are carefully selected to ensure
        that they meet our high standards of quality.</p>

    <h2>Contact Us</h2>
    <p>If you have any questions or concerns, please feel free to contact us. You can reach us by phone at (123)
        456-7890 or by email at info@ourcompany.com. We look forward to hearing from you!</p>

    <h2>developers information</h2>
    
    <!-- Add Dev1 name here -->
    <p>Dev1 name: <br>Dev2 name: </p>
    
</body>

</html>
  ```
  
</details>

<details>
  <summary>
    Div1 links the details.html with index.html in the navbar
  </summary>
  
  ```html
  [old]
  <li><a href="#about">About</a></li>
  [new]
  <li><a href="about.html">About</a></li>
  ```
  
</details>

<details>
  <summary>
    Div2 creates "about_styles.css" file with the following styles
  </summary>
  
  ```css
  p {
    color: brown;
}

h2 {
    color: crimson;
}
  ```
  
</details>

<details>
  <summary>
    Div1 links the "about_styles.css" in "about.html" page 
  </summary>
  
  ```html
  <link rel="stylesheet" type="text/css" href="about_styles.css"/>
  ```
  
</details>

<details>
  <summary>
    Div1 adds their name in "Dev1 name: " paragraph
  </summary>
  
  ```html
  <p>Dev1 name: YOUR_NAME</p>
  ```
  
</details>

<details>
  <summary>
    Div2 adds their name in "Dev2 name: " paragraph
  </summary>
  
  ```html
  <p><br>Dev2 name: YOUR_NAME</p>
  ```
  
</details><br>

### Open an issue
Div2 notices that in "index.html", the h1 title is Git & GitHub assignment #2 :)  
Since Div1 is the one who created this file they will get the blame :P 
<details>
  <summary>
    Div2 opens an issue in "issues" tab and inform Div1 about that issue
  </summary>
  
  ```
  [Example]
  Hello Div1,
  Please fix the issue found at "index.html" page where the h1 tag shows "Git & GitHub assignment #1", while we are still in assignment #! :)
  ```
  
</details>

<details>
  <summary>
    Div1 solves the issue by fixing the title in the h1 tag, then informs the issuer and closes the issue.
  </summary>
  
  ```html
<h1>Git & GitHub assignment #1</h1>
  ```
  
</details><br>

### Deploy the website on GitHub pages
- Div1 deploys the "index.html" by going to (settings -> pages) then choose master as deployment branch
- Div2 verifies the url found in (settings -> pages) after a successful deployment.
- Div1 unpublishes the site since they found some issues they need to fix. (settings -> pages -> burger icon -> unpublish)
