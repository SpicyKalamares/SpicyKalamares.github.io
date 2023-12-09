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
  </style>
</head>
<body>
  <h1>My GitHub Repositories</h1>
  <ul id="repositories-list">
    <li>
      <h2>Prelim Period</h2>
      <ul id="prelim-repositories-list"></ul>
      <h3>Prelim Exam</h3>
      <ul id="prelimexam-repositories-list"></ul>
    </li>
    <li>
      <h2>Midterm Period</h2>
      <ul id="midterm-repositories-list"></ul>
      <h3>Midterm Exam</h3>
      <ul id="midtermexam-repositories-list"></ul>
    </li>
    <li>
      <h2>Final Period</h2>
      <ul id="final-repositories-list"></ul>
    </li>
      <h1>Relection and Learning from the course</h1>
        <h4>  After takin this course </h4>
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

    // Display the specified repositories for Prelim Period
    const prelimRepositoriesList = document.getElementById('prelim-repositories-list');
    const prelimExamRepositoriesList = document.getElementById('prelimexam-repositories-list');

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

    // Display the specified repositories for Midterm Period
    const midtermRepositoriesList = document.getElementById('midterm-repositories-list');
    const midtermExamRepositoriesList = document.getElementById('midtermexam-repositories-list');

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

    // Display the specified repositories for Final Period
    const finalRepositoriesList = document.getElementById('final-repositories-list');
    const finalExamRepositoriesList = document.getElementById('finalexam-repositories-list');

    finalRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      finalRepositoriesList.appendChild(listItem);
    });
  </script>
</body>
</html>
