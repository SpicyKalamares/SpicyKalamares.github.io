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
  <ul id="repositories-list"></ul>

  <script>
    // Replace 'your-username' with your GitHub username
    const username = 'your-username';

    // Fetch GitHub repositories
    fetch(`https://api.github.com/users/${username}/repos`)
      .then(response => response.json())
      .then(repositories => {
        const repositoriesList = document.getElementById('repositories-list');

        repositories.forEach(repo => {
          const listItem = document.createElement('li');
          const link = document.createElement('a');

          link.href = repo.html_url;
          link.textContent = repo.name;

          listItem.appendChild(link);
          repositoriesList.appendChild(listItem);
        });
      })
      .catch(error => {
        console.error('Error fetching GitHub repositories:', error);
      });
  </script>
</body>
</html>
