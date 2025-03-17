# grid-cloud-task1
# Task 1. Basics of containerization
    
This project demonstrates a simple UI with PostgeSQL running in Docker containers.
## Setup and Run</h2>
<ol>
    <li>Precondition: you have docker installed.</li>
    <li>Clone the repository:</li>
    <pre><code>git clone https://github.com/polinaantropova/grid-cloud-task1.git </code></pre>
    <li>Navigate to the project folder:</li>
    <pre><code>cd &lt;repo_folder&gt;</code></pre>
    <li>Build and start the containers:</li>
    <pre><code>docker-compose up</code></pre>
    <li>UI will be available at:</li>
    <pre><code>http://localhost:8080</code></pre>
</ol>

## Testing container collaboration
To confirm that PostgreSQL data persists after restarting containers:

1. Login the UI Adminer:
Use the image as a sample to fill in. The password can be found in the file's environment variable of the docker-compose.yml

![image](https://github.com/polinaantropova/grid-cloud-task1/blob/main/images/1.png)

2. Create a new table:
For example test_table with ID(integer not null) and text(text).
            
![image](https://github.com/user-attachments/assets/551b29a6-9d07-49d3-a069-5f8e884036fd)
        
3. Edit the table, add new entry:
For example, add some strings: (1, 'first'), (2, 'second').
        
![image](https://github.com/polinaantropova/grid-cloud-task1/blob/main/images/3.jpg)
        
4. Stop the docker-compose:
<pre><code>docker-compose down</code></pre>
5. Build and start the containers:
<pre><code>docker-compose up</code></pre>
6. Login the UI Adminer (look at step 1)
7. Go to test_table.
If the table contains records that were created during the previous container run, it means that the database is persistent in this build.

![image](https://github.com/polinaantropova/grid-cloud-task1/blob/main/images/4.jpg)

