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
    .dropdown-toggle:hover + .dropdown,
    .dropdown:hover {
      display: block;
    }
  </style>
</head>
<body>
  <h1>My GitHub Repositories</h1>
  <ul id="repositories-list">
    <li>
      <i class="fas fa-code icon"></i>
      <h2 class="dropdown-toggle" id="prelim-period">Prelim Period</h2>
      <ul class="dropdown" id="prelim-dropdown">
        <li>
          <h3>Prelim Exam</h3>
          <ul id="prelimexam-repositories-list"></ul>
        </li>
      </ul>
      <ul id="prelim-repositories-list"></ul>
    </li>
    <li>
      <i class="fas fa-code icon"></i>
      <h2 class="dropdown-toggle" id="midterm-period">Midterm Period</h2>
      <ul class="dropdown" id="midterm-dropdown">
        <li>
          <h3>Midterm Exam</h3>
          <ul id="midtermexam-repositories-list"></ul>
        </li>
      </ul>
      <ul id="midterm-repositories-list"></ul>
    </li>
    <li>
      <i class="fas fa-code icon"></i>
      <h2 class="dropdown-toggle" id="final-period">Final Period</h2>
      <ul class="dropdown" id="final-dropdown">
        <li>
          <h3>Final Exam</h3>
          <ul id="finalexam-repositories-list"></ul>
        </li>
      </ul>
      <ul id="final-repositories-list"></ul>
    </li>
    <li>
      <h1>Reflection and Learning from the course</h1>
      <h4>After taking this course</h4>
    </li>
  </ul>

  <script>
    const username = 'SpicyKalamares';

    const prelimRepositories = [
      'CPE232_HOA1',
      'CPE232_HOA2',
      'CPE232_HOA3',
      'CPE232_HOA4',
      'CPE232_HOA5'
    ];

    const midtermRepositories = [
      'CPE232_HOA6',
      'CPE232_HOA7',
      'CPE232_HOA8',
      'CPE232_HOA9',
      'CPE232_HOA10'
    ];

    const finalRepositories = [
      'CPE232_HOA11',
      'CPE232_HOA12',
      'CPE232_HOA13',
      'CPE232_HOA14',
      'CPE232_HOA15'
    ];

    const prelimExamRepositories = [
      'Reyes_PrelimExam'
    ];

    const midtermExamRepositories = [
      'Reyes_MidtermExam'
    ];

    const finalExamRepositories = [
      'Reyes_FinalExam'
    ];

    // Display the specified repositories for Prelim Period
    const prelimRepositoriesList = document.getElementById('prelim-repositories-list');
    const prelimExamRepositoriesList = document.getElementById('prelimexam-repositories-list');
    const prelimDropdown = document.getElementById('prelim-dropdown');

    prelimRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      prelimRepositoriesList.appendChild(listItem);
    });

    prelimExamRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      prelimExamRepositoriesList.appendChild(listItem);
    });

    // Add click event listener to Prelim Period header
    document.getElementById('prelim-period').addEventListener('click', function() {
      // Toggle the visibility of the Prelim repositories list
      prelimDropdown.style.display = prelimDropdown.style.display === 'none' ? 'block' : 'none';
    });

    // Display the specified repositories for Midterm Period
    const midtermRepositoriesList = document.getElementById('midterm-repositories-list');
    const midtermExamRepositoriesList = document.getElementById('midtermexam-repositories-list');
    const midtermDropdown = document.getElementById('midterm-dropdown');

    midtermRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      midtermRepositoriesList.appendChild(listItem);
    });

    midtermExamRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      midtermExamRepositoriesList.appendChild(listItem);
    });

    // Add click event listener to Midterm Period header
    document.getElementById('midterm-period').addEventListener('click', function() {
      // Toggle the visibility of the Midterm repositories list
      midtermDropdown.style.display = midtermDropdown.style.display === 'none' ? 'block' : 'none';
    });

    // Display the specified repositories for Final Period
    const finalRepositoriesList = document.getElementById('final-repositories-list');
    const finalExamRepositoriesList = document.getElementById('finalexam-repositories-list');
    const finalDropdown = document.getElementById('final-dropdown');

    finalRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      finalRepositoriesList.appendChild(listItem);
    });

    finalExamRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      finalExamRepositoriesList.appendChild(listItem);
    });

    // Add click event listener to Final Period header
    document.getElementById('final-period').addEventListener('click', function() {
      // Toggle the visibility of the Final repositories list
      finalDropdown.style.display = finalDropdown.style.display === 'none' ? 'block' : 'none';
    });
  </script>
</body>
</html>
