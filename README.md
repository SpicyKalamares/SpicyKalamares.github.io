<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My GitHub Repositories</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 20px;
    }
    h1 {
      color: #333;
    }
    ul {
      list-style-type: none;
      padding: 0;
    }
    li {
      margin-bottom: 10px;
    }
    a {
      text-decoration: none;
      color: #0366d6;
    }
  </style>
</head>
<body>
  <h1>My GitHub Repositories</h1>
  <ul id="repositories-list">
    <li>
      <h2>Prelim Period</h2>
      <ul id="prelim-repositories-list"></ul>
    </li>
  </ul>

  <script>
    const username = 'SpicyKalamares';

    const prelimRepositories = [
      'CPE232_HOA1',
      'CPE232_HOA2',
      'CPE232_HOA3'
      // Add more repositories as needed
    ];

    // Display the specified repositories
    const prelimRepositoriesList = document.getElementById('prelim-repositories-list');

    prelimRepositories.forEach(repoName => {
      const listItem = document.createElement('li');
      const link = document.createElement('a');

      link.href = `https://github.com/${username}/${repoName}`;
      link.textContent = repoName;

      listItem.appendChild(link);
      prelimRepositoriesList.appendChild(listItem);
    });
  </script>
</body>
</html>
