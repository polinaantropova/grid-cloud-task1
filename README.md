# grid-cloud-task1

<body>
    <h1>Task 1. Basics of containerization</h1>
    <p>This project demonstrates a simple UI with PostgeSQL running in Docker containers.</p>
    <h2>Setup and Run</h2>
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
    <h2>Testing container collaboration</h2>
    <p>To confirm that PostgreSQL data persists after restarting containers:</p>
    <ol>
        <li>Login the UI Adminer:</li>
        <p>Use the image as a sample to fill in. The password can be found in the file's environment variable of the docker-compose.yml</p>
        ![image](https://github.com/user-attachments/assets/d71baba3-3a25-4d41-a8eb-6937acaa74d7)
        <li>Create a new table:</li>
        <p>For example table_1 with ID(integer not null) and text(text).<p>
        ![image](https://github.com/user-attachments/assets/551b29a6-9d07-49d3-a069-5f8e884036fd)
    </ol>
</body>
</html>
