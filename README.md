<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Task Management Tool</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>Task Management Tool</h1>
    <nav>
      <a href="#projects">Projects</a>
      <a href="#team">Team</a>
      <a href="#tasks">Tasks</a>
    </nav>
  </header>

  <section id="projects">
    <h2>Projects</h2>
    <div class="project-list">
      <div class="project-card">
        <h3>Project A</h3>
        <p>Status: In Progress</p>
        <button onclick="viewProject(1)">View Details</button>
      </div>
      <div class="project-card">
        <h3>Project B</h3>
        <p>Status: Completed</p>
        <button onclick="viewProject(2)">View Details</button>
      </div>
    </div>
    <button onclick="createProject()">Create New Project</button>
  </section>

  <section id="team">
    <h2>Team</h2>
    <div class="team-member">
      <h3>Nitin kumar</h3>
      <p>Role: Manager</p>
    </div>
    <div class="team-member">
      <h3>Abhishek Singh</h3>
      <p>Role: Team Lead</p>
    </div>
    <div class="team-member">
      <h3>Aryan Sharma</h3>
      <p>Role: Developer</p>
    </div>
  </section>

  <section id="tasks">
    <h2>Tasks</h2>
    <div class="task-list">
      <div class="task-card">
        <h3>Task 1</h3>
        <p>Assigned to: Nitin kumar</p>
        <p>Status: In Progress</p>
        <button onclick="updateTask(1)">Update Status</button>
      </div>
      <div class="task-card">
        <h3>Task 2</h3>
        <p>Assigned to: Abhishek Singh</p>
        <p>Status: Pending</p>
        <button onclick="updateTask(2)">Update Status</button>
      </div>
    </div>
  </section>

  <!-- Modal for creating new project -->
  <div id="create-project-modal" class="modal">
    <div class="modal-content">
      <h2>Create New Project</h2>
      <label for="project-name">Project Name:</label>
      <input type="text" id="project-name" placeholder="Enter project name">
      <button onclick="saveProject()">Save Project</button>
      <button onclick="closeModal()">Cancel</button>
    </div>
  </div>

  <script src="app.js"></script>
</body>
</html>
