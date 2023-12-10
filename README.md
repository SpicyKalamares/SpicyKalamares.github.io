<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My GitHub Repositories</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
  <style>
    body {
      font-family: 'Arial', sans-serif;
      margin: 20px;
      background-color: #f8f9fa;
    }
    h1 {
      color: #0366d6;
    }
    ul {
      list-style-type: none;
      padding: 0;
    }
    li {
      margin-bottom: 15px;
      background-color: #fff;
      padding: 10px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      transition: background-color 0.3s ease;
    }
    li:hover {
      background-color: #f1f1f1;
    }
    a {
      text-decoration: none;
      color: #0366d6;
      transition: color 0.3s ease;
    }
    a:hover {
      color: #1a0dab;
    }
    .icon {
      margin-right: 8px;
    }
    .dropdown {
      display: none;
      margin-top: 10px;
    }
    .dropdown-btn {
      background-color: #0366d6;
      color: #ffffff;
      padding: 5px 10px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    .dropdown-btn:hover {
      background-color: #1a0dab;
    }
    .dropdown-arrow::after {
      content: " ▼"; /* Unicode character for down arrow */
    }
  </style>
</head>
<body>
  <h1>CPE232 - Managing Enterprise Servers</h1>
  <ul id="repositories-list">
    <li>
      <i class="fas fa-code icon"></i>
      <button class="dropdown-btn dropdown-arrow" id="prelim-period">Prelim Period</button>
      <ul class="dropdown" id="prelim-dropdown">
        <!-- Placeholder for Prelim repositories -->
      </ul>
    </li>
    <li>
      <i class="fas fa-code icon"></i>
      <button class="dropdown-btn dropdown-arrow" id="midterm-period">Midterm Period</button>
      <ul class="dropdown" id="midterm-dropdown">
        <!-- Placeholder for Midterm repositories -->
      </ul>
    </li>
    <li>
      <i class="fas fa-code icon"></i>
      <button class="dropdown-btn dropdown-arrow" id="final-period">Final Period</button>
      <ul class="dropdown" id="final-dropdown">
        <!-- Placeholder for Final repositories -->
      </ul>
    </li>
    <li>
      <h1>Reflection and Learning from the course</h1>
      <h4>After taking this course</h4>
    </li>
  </ul>

  <script>
    const username = 'SpicyKalamares';

    const prelimExamRepositories = ['CPE232_HOA1', 'CPE232_HOA2', 'CPE232_HOA3', 'CPE232_HOA4', 'CPE232_HOA5'];
    const midtermExamRepositories = ['CPE232_HOA6', 'CPE232_HOA7', 'CPE232_HOA8', 'CPE232_HOA9', 'CPE232_HOA10'];
    const finalExamRepositories = ['CPE232_HOA11', 'CPE232_HOA12', 'CPE232_HOA13', 'CPE232_HOA14', 'CPE232_HOA15'];

    // Display the specified repositories for Prelim Period
    const prelimExamRepositoriesList = document.getElementById('prelim-dropdown');

    prelimExamRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      prelimExamRepositoriesList.appendChild(listItem);
    });

    // Add click event listener to Prelim Period button
    document.getElementById('prelim-period').addEventListener('click', function() {
      // Toggle the visibility of the Prelim repositories list
      prelimExamRepositoriesList.style.display = prelimExamRepositoriesList.style.display === 'none' ? 'block' : 'none';
    });

    // Display the specified repositories for Midterm Period
    const midtermExamRepositoriesList = document.getElementById('midterm-dropdown');

    midtermExamRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      midtermExamRepositoriesList.appendChild(listItem);
    });

    // Add click event listener to Midterm Period button
    document.getElementById('midterm-period').addEventListener('click', function() {
      // Toggle the visibility of the Midterm repositories list
      midtermExamRepositoriesList.style.display = midtermExamRepositoriesList.style.display === 'none' ? 'block' : 'none';
    });

    // Display the specified repositories for Final Period
    const finalExamRepositoriesList = document.getElementById('final-dropdown');

    finalExamRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      finalExamRepositoriesList.appendChild(listItem);
    });

    // Add click event listener to Final Period button
    document.getElementById('final-period').addEventListener('click', function() {
      // Toggle the visibility of the Final repositories list
      finalExamRepositoriesList.style.display = finalExamRepositoriesList.style.display === 'none' ? 'block' : 'none';
    });
  </script>
</body>
</html>
