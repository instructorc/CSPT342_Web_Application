# CPST 342 Group Project Repository 

You will complete three assignments that will culminate in developing a monolithic full-stack web application. 

For the first group assignment, you will propose what type of app you will build and use the README.md file to document your responses to the questions for Assignment 1 deliverable 1.  All documentation pertaining to your project should occur in the README.md. 

After this course, your application will consist of the following components listed below.

1. Routing Framework using Express.js
2. Demonstrate and utilize a REST API
3. Create, Retrieve, Update and Delete (CRUD) Functionality
4. Utilize SQLite Database for persistent data store
5. Functional and User-friendly front-end interface
6. Hosting that allows users to access the site via domain name
7. Accessibility and Usability Considerations

**Assignment 1 consist of deliverables 1 and 2** <br>
**Assignment 2 consist of deliverables  3 and 4** <br>
**Assignment 3 consist of deliverables 5, 6, and 7** <br>


## Assignment 1  - Project proposal
### Deliverable 1 (15 Points)
For this deliverable, you will need to modify the readme file and add responses to the questions below. that you are currently reading and address the following items below using a variety of permissible markdown syntax.

- Provide your name or the team's name
- Name of the application
- Description of application *Describe how someone will use your application
- Describe the need and purpose of the application
- Intended target audience
- Identify the various pages your application will have and describe what users will be able to accomplish
- Identify three goals of the application
- Identify tools/software you will use to complete the project. 
* I suggest using an online coding environment that will allow your team to work collaboratively and practice git commands.  A few are listed below.
   - [Codeeverywhere.com](https://codeeverywhere.com)
   - [Replit.com](https://replit.com/)

### Deliverable 2 - Version control (15 Points)
For this deliverable, you will implement version control in your project folder. The purpose of this deliverable is to provide an opportunity to practice using git in such a way that allows you to document and capture incremental progress. If working as a team, you will need to practice as a team editing the README.md file with each team member making a series of commits. If you are completing the project solo, consider incrementally making commits to achieve the requirements of deliverable I.
- Your remote repository will need to contain a minimum of 2 commits from each member for assignment 1 
- [For Teams] Your remote repository must include at least two commits from each team member for Assignment 1 
- [If completing Solo] Your remote repository must include at least five commits displaying your incremental progress. 


### Assignment 1 Rubric

#### Deliverable 1 - Project proposal (15 Points)
| Criteria | Description | Points |
| --- | --- | ---: |
| Team and application identity | Provides the team or student name and application name. | 2 |
| Application description and purpose | Explains what the application does, how it will be used, and the need it addresses. | 4 |
| Target audience | Identifies the intended users. | 2 |
| Pages and user activities | Lists the planned pages and describes what users can accomplish on each. | 3 |
| Application goals | Identifies three goals for the application. | 2 |
| Tools and software | Identifies the tools and software planned for the project. | 2 |
| **Total Points** |  | **15** |

#### Deliverable 2 - Version control (15 Points)
| Criteria | Description | Points |
| --- | --- | ---: |
| Remote repository | Project is available in the assigned remote repository. | 3 |
| Commit requirement | Team projects contain at least two commits from each member; solo projects contain at least five commits. | 8 |
| Incremental progress | Commits document incremental project progress, including work toward Deliverable 1. | 4 |
| **Total Points** |  | **15** |

**Assignment 1 Total: 30 Points**

## Assignment 2 - Express Routing + CRUD Operations using SQLite Database.

### Deliverable 3 - Routing and Middleware configuration (15 Points)
For this deliverable, you will focus on implementing the necessary middleware needed to configure and route your application. Feel free to refer back to the [node.js](https://instructorc.github.io/site/slides/logic/nodejs.html) presentation for code samples and an explanation of concepts.
- Middleware is implemented for static files such as images, pdf's, etc (2 points)
- Middleware is implemented for view templating engine (2 points)
- Middleware configured to parse JSON data and interpret form data.  Implement the following code below to meet requirement. (2 points)
``` javascript
 // parse application/json
app.use(express.json());

// For parsing application/x-www-form-urlencoded
app.use(express.urlencoded({ extended: true }));
```

- Application has a minimum of 5 routes implemented 
  1.  A minimum of three routes should accept data. Both the GET and POST methods will need to be represented in your routing functions (5 points)
     1. At a minimum one route should make a call to an external REST API
  2.  A minimum of three routes should render data back to the client/user interface. (4 points)
     1. At a minimum one route should return JSON data from external REST API to the interface
 
 

### Deliverable 4 - Database implementation (15 Points)
- Your application contains a file titled "database.js" and all of your SQL queries are listed and identified. (2 points)
- Your database.js file contains a minimum of 4 queries that represent the Create, Retrieve, Update and Delete (CRUD) functionality. (8 points)
- Database queries are represented within the routes and perform CRUD operations. (2 points)
- SQLite Database file is included within the project folder  (3 points)

### Assignment 2 Rubric

#### Deliverable 3 - Routing and middleware configuration (15 Points)
| Criteria | Description | Points |
| --- | --- | ---: |
| Static-file middleware | Configures middleware to serve static files such as images or PDFs. | 2 |
| View templating middleware | Configures a view templating engine. | 2 |
| Request-body parsing | Configures middleware to parse JSON and URL-encoded form data. | 2 |
| Routes and accepted data | Implements at least five routes, including at least three routes that accept data and use both GET and POST methods; at least one route calls an external REST API. | 5 |
| Routes rendering data | Implements at least three routes that render data to the interface, including one that returns external REST API JSON data to the interface. | 4 |
| **Total Points** |  | **15** |

#### Deliverable 4 - Database implementation (15 Points)
| Criteria | Description | Points |
| --- | --- | ---: |
| Database query file | Includes a `database.js` file with SQL queries listed and identified. | 2 |
| CRUD queries | Includes at least four database queries covering Create, Retrieve, Update, and Delete. | 8 |
| Queries used by routes | Uses database queries within routes to perform CRUD operations. | 2 |
| SQLite database file | Includes the SQLite database file in the project folder. | 3 |
| **Total Points** |  | **15** |

**Assignment 2 Total: 30 Points**

## Assignment 3 - Finalizing User-Interface and Hosting Site

### Deliverable 5 - Functional and User-Friendly front-end interface (10 Points)

For this deliverable, you will need to make sure each of the pages of your site are properly functioning and renders in the browser.  Listed below are items that should be identified in your app. 

- Interface uses HTML form(s) to capture data that is related to CREATE and UPDATE functionality. (5 Points)
- Interface displays data that is queried from the database (3 Points)
- Interface includes a home page that is mapped to the root directory of your project folder.  For example, your web application should have a route that listens for the URL path of “/” and returns the homepage. (2 Points)

### Deliverable 6 - Hosting Site (10 Points)

For this deliverable, your group will deploy and host your site on Heroku.  The service cost $5 a month for an Eco dynos.  Information regarding cost can be found at this [link](https://www.heroku.com/pricing#containers) 
I recommend all group members pitch in a few dollars to host the site for 1 month.
Heroku - [https://www.heroku.com](https://www.heroku.com/)  

Only one member of your team will need to create an account. 
Heroku will need to be configured to host your site from the GitHub repository issued by the instructor. 

Update the repository Readme file to include the URL from Heroku

### Deliverable 7 - Usability and accessibility (10 Points)

Evaluate and improve the application's user experience using Jakob Nielsen's 10 usability heuristics. Review each user-facing page and key task flow, and document usability issues found and the changes made to address them.

1. Visibility of system status
2. Match between the system and the real world
3. User control and freedom
4. Consistency and standards
5. Error prevention
6. Recognition rather than recall
7. Flexibility and efficiency of use
8. Aesthetic and minimalist design
9. Help users recognize, diagnose, and recover from errors
10. Help and documentation

Use semantic HTML and native elements first. Add ARIA roles, accessible names, states, and properties where needed to communicate interface semantics to assistive technology; do not use ARIA to replace semantics already provided by native elements. The site must meet WCAG 2.2 Level AA requirements, including keyboard access, visible focus, sufficient contrast, text alternatives, labeled form controls, and accessible error feedback.

### Assignment 3 Rubric

#### Deliverable 5 - Functional and user-friendly front-end interface (10 Points)
| Criteria | Description | Points |
| --- | --- | ---: |
| Create and update forms | Uses HTML forms to capture data for Create and Update functionality. | 5 |
| Database results | Displays data queried from the database. | 3 |
| Home page route | Provides a home page at the root URL (`/`). | 2 |
| **Total Points** |  | **10** |

#### Deliverable 6 - Hosting site (10 Points)
| Criteria | Description | Points |
| --- | --- | ---: |
| Hosted application | Deploys the application to Heroku and makes it accessible. | 5 |
| Repository configuration | Configures Heroku to host the site from the instructor-issued GitHub repository. | 3 |
| README deployment URL | Adds the Heroku application URL to the repository README. | 2 |
| **Total Points** |  | **10** |

#### Deliverable 7 - Usability and accessibility (10 Points)
| Criteria | Description | Points |
| --- | --- | ---: |
| Nielsen's usability heuristics | Reviews key pages and task flows against all 10 heuristics and documents identified issues and improvements. | 4 |
| Accessible semantics and ARIA | Uses semantic HTML and appropriate ARIA roles, names, states, and properties without duplicating native semantics. | 2 |
| WCAG 2.2 Level AA | Meets Level AA requirements, including keyboard access, visible focus, contrast, text alternatives, labeled controls, and accessible error feedback. | 4 |
| **Total Points** |  | **10** |

**Assignment 3 Total: 30 Points**


### Extra Credit – Implementing Authentication + Authorization using Passport.js or a third-party authentication tool (7 Extra Credit Points)

Once requirements from deliverable 1 -6 are met and and your group would like an additional challenge then I would encourage you to consider implementing an authentication library called passport.js or implementing a third-party authentication service such as AuthO (https://auth0.com/) or Stytch (https://stytch.com/). To successfully meet the requirements for extra credit, you will need to adhere to the following bullet points below. All the following requirements will need to be met to receive full credit. 

- Implementation of authentication should flow succinctly with the rest of your applicaiton and not be disjointed and unpurposeful.
- Once an account is successfully created, the end user will be directed to a welcome screen connects account to a dashboard or user profile page.
- Once a user logs out, the end user is notified they are logged out of the application and redirected to another page.
  
### Submission Guidelines
Your project folder will need to be submitted to the assigned GitHub repository provided to you by the instructor. In Sakai, you will need to submit the link to your repository by the due date and time listed in the write-up. Make sure you receive confirmation from Sakai that your assignment has been submitted.

## Resources
[Markdown Syntax CheatSheet](https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf)
