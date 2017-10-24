# Milestones List  
  
### Basic Scaffolding Milestone  
The first milestone for our project is to finish all basic scaffolding required to get into the thick of the development work for this project. This milestone includes researching the Triton DataCenter API endpoints to decide on what features we can add and how we will communicate them from our application to the physical server running Triton DataCenter. This milestone also includes researching and deciding on what frontend, backend, and database frameworks we will use to complete this project. Finally, this milestone will also include the basic program and files to begin unit testing, which we will add to throughout the course of this project.  
  
### Basic Web Application Milestone  
The second milestone of our project is to finish all of the basic page creation and have it up and ready to be tested in our QA environment. The first part of this milestone is to create the basic design template for what we want the application to look like. The next steps are to create the signup page and it’s controller, along with its service and backend controller. The same will be done for the login page.  
  
### Advanced Web Application Milestone  
The third milestone is to finish the more advanced sections of our web application. This includes creating the default account management page, which includes an account information section, and sections to edit the network list, image list, and current virtual machine instances, along with a controller, service, and a backend controller.  
  
### Connections Milestone  
The fourth milestone is to tie everything together by connecting the backend controllers to the Triton DataCenter API and a PostgresSQL database. This milestone is the final step to our application being usable. In this step, we will finish the backend service that connects the data from the frontend of our application and sends it to be saved in either Triton DataCenter or our PostgresSQL database.  
  
# Timeline
|Task number|Task|Start Date|End Date|Milestone|Predecessor(s)|Spencer Effort|Matt Effort|Alec Effort|
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
|1|Research Triton DataCenter API endpoints|10/25/17|10/27/17|1|-|33%|33%|33%|
|2|Decide on frontend/backend/database frameworks for use|10/30/17|10/31/17|1|-|33%|33%|33%|
|4|Create basic design template for whole application|11/6/17|11/10/17|2|-|80%|10%|10%|
|5|Create signup page and controller|11/13/17|11/15/17|2|4|15%|15%|70%|
|6|Create login page and controller|11/15/17|11/17/17|2|4|25%|50%|25%|
|7|Create default account management page - Account details and edit section|11/20/17|11/24/17|3|5,6|60%|20%|20%|
|8|Create network list management section on account management page|11/27/17|12/1/17|3|5,6,7|15%|15%|70%|
|9|Create image list management section on account management page|12/4/17|12/8/17|3|5,6,7|25%|55%|20%|
|10|Create virtual machine instances list section on account management page |12/11/17|12/15/17|3|5,6,7|60%|15%|25%|
|11|Create service to connect changes on frontend to the Triton DataCenter API|12/18/17|12/22/17|4|5,6,7|15%|20%|65%|
|12|Create service to connect account detail changes to PostgresSQL database|12/26/17|12/29/17|4|5,6,7|10%|75%|15%|

# Effort Matrix
![Effort Matrix](https://github.com/dangelspencer/skyline/blob/master/timeline/effort_matrix.png)
