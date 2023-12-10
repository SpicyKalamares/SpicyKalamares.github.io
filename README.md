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
      content: " ▼";
      /* Unicode character for down arrow */
    }

    .dropdown-header {
      font-weight: bold;
      margin-bottom: 8px;
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
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA1">CPE232_HOA1</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA2">CPE232_HOA2</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA3">CPE232_HOA3</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA4">CPE232_HOA4</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA5">CPE232_HOA5</a>
        </li>
        <!-- Include Prelim Exam in the Prelim Period dropdown -->
        <li class="dropdown-header">Prelim Exam</li>
        <li>
          <a href="https://github.com/SpicyKalamares/Reyes_PrelimExam">Reyes_PrelimExam</a>
        </li>
      </ul>
    </li>
    <li>
      <i class="fas fa-code icon"></i>
      <button class="dropdown-btn dropdown-arrow" id="midterm-period">Midterm Period</button>
      <ul class="dropdown" id="midterm-dropdown">
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA6">CPE232_HOA6</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA7">CPE232_HOA7</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA8">CPE232_HOA8</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA9">CPE232_HOA9</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA10">CPE232_HOA10</a>
        </li>
        <!-- Include Midterm Exam in the Midterm Period dropdown -->
        <li class="dropdown-header">Midterm Exam</li>
        <li>
          <a href="https://github.com/SpicyKalamares/Reyes_MidtermExam">Reyes_MidtermExam</a>
        </li>
      </ul>
    </li>
    <li>
      <i class="fas fa-code icon"></i>
      <button class="dropdown-btn dropdown-arrow" id="final-period">Final Period</button>
      <ul class="dropdown" id="final-dropdown"></ul>
    </li>
    <li>
      <h1>Reflection and Learning from the course</h1>
      <h4>After taking this course</h4>
    </li>
  </ul>

  <script>
    document.addEventListener('DOMContentLoaded', function () {
      const username = 'SpicyKalamares';

      const finalRepositories = [
        'CPE232_HOA11',
        'CPE232_HOA12',
        'CPE232_HOA13',
        'CPE232_HOA14',
        'CPE232_HOA15',
        'Reyes_FinalExam'
      ];

      // Display the specified repositories for Final Period
      const finalRepositoriesList = document.getElementById('final-dropdown');
      finalRepositories.forEach(repoName => {
        const listItem = document.createElement('li');
        const link = document.createElement('a');

        link.href = `https://github.com/${username}/${repoName}`;
        link.textContent = repoName;

        listItem.appendChild(link);
        finalRepositoriesList.appendChild(listItem);
      });

      // Add click event listener to Final Period button
      document.getElementById('final-period').addEventListener('click', function () {
        // Toggle the visibility of the Final repositories list
        finalRepositoriesList.style.display = finalRepositoriesList.style.display === 'none' ? 'block' : 'none';
      });
    });

    // Add click event listener to Prelim Period button
    document.getElementById('prelim-period').addEventListener('click', function () {
      // Toggle the visibility of the Prelim repositories list
      const prelimDropdown = document.getElementById('prelim-dropdown');
      prelimDropdown.style.display = prelimDropdown.style.display === 'none' ? 'block' : 'none';
    });

    // Add click event listener to Midterm Period button
    document.getElementById('midterm-period').addEventListener('click', function () {
      // Toggle the visibility of the Midterm repositories list
      const midtermDropdown = document.getElementById('midterm-dropdown');
      midtermDropdown.style.display = midtermDropdown.style.display === 'none' ? 'block' : 'none';
    });
  </script>
</body>

</html>
