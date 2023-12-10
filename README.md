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
      background: url(https://e0.pxfuel.com/wallpapers/739/45/desktop-wallpaper-server-room-servers.jpg) center/cover no-repeat;
    }

    h1 {
      color: #ffffff;
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
      border-radius: 0;
      cursor: pointer;
      transition: background-color 0.3s ease;
      outline: none;
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
      <i class="fas fa-square icon"></i>
      <button class="dropdown-btn dropdown-arrow" id="prelim-period">Prelim Period</button>
      <ul class="dropdown" id="prelim-dropdown">
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA1">CPE232_HOA1 - Creating Virtual Machine</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA2">CPE232_HOA2 - SSH Key-Based Authentication and GIT Setup</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA3">CPE232_HOA3 - Install SSH server on CentOS or RHEL 8</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA4">CPE232_HOA4 - Ansible Basics</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA5">CPE232_HOA5 - Implement Ansible Roles in Playbook</a>
        </li>
        <!-- Include Prelim Exam in the Prelim Period dropdown -->
        <li class="dropdown-header">Prelim Exam</li>
        <li>
          <a href="https://github.com/SpicyKalamares/Reyes_PrelimExam">Reyes_PrelimExam</a>
        </li>
      </ul>
    </li>
    <li>
      <i class="fas fa-square icon"></i>
      <button class="dropdown-btn dropdown-arrow" id="midterm-period">Midterm Period</button>
      <ul class="dropdown" id="midterm-dropdown">
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA6">CPE232_HOA6 - Targeting Specific Nodes</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA7">CPE232_HOA7 - Managing Files and Creating Roles in Ansible</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA8">CPE232_HOA8 - Install, Configure, and Manage Enterprise Availability Monitoring via Ansible</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA9">CPE232_HOA9 - Install, Configure, and Manage Enterprise Availability Performance via Ansible</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA10">CPE232_HOA10 - Install, Configure, and Manage Enterprise Log Monitoring via Ansible</a>
        </li>
        <!-- Include Midterm Exam in the Midterm Period dropdown -->
        <li class="dropdown-header">Midterm Exam</li>
        <li>
          <a href="https://github.com/SpicyKalamares/Reyes_MidtermExam">Reyes_MidtermExam</a>
        </li>
      </ul>
    </li>
    <li>
      <i class="fas fa-square icon"></i>
      <button class="dropdown-btn dropdown-arrow" id="final-period">Final Period</button>
      <ul class="dropdown" id="final-dropdown">
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA11">CPE232_HOA11 - Containerization</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA12">CPE232_HOA12 - Build a Sample Web App in a Docker Container</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA13">CPE232_HOA13 - OpenStack Prerequisite Installation</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA14">CPE232_HOA14 - OpenStack Installation (Keystone, Glance, Nova)</a>
        </li>
        <li>
          <a href="https://github.com/SpicyKalamares/CPE232_HOA15">CPE232_HOA15 - OpenStack Installation (Neutron, Horizon, Cinder)</a>
        </li>
      </ul>
    </li>
    <li>
      <h2>Reflection and Learning from the Course</h2>
      <h4>After taking this course, I was able to learn the basics of ansible and how important it is when there is a large number of servers in an enterprise. This makes the admin's work easy as they can install or update every server using one host only and this makes a good time management. Having this as an advantage, there is also a disadvantage where it requires a medium to high specification system to sustain all the process that the ansible will do to the servers. Now that the course comes to an end, i learned many  things such as making the codes and running it via ansible. Understanding the codes will be used so that I can explore how my codes work and I can easily find the errors that I encountered. With this course, I am able to have the skills that I can use as a computer engineering student. </h4>
    </li>
  </ul>

  <script>
    document.addEventListener('DOMContentLoaded', function () {
      const username = 'SpicyKalamares';

      // Display the specified repositories for Final Period
      const finalRepositoriesList = document.getElementById('final-dropdown');
      finalRepositoriesList.style.display = 'none';

      // Add click event listener to Final Period button
      document.getElementById('final-period').addEventListener('click', function () {
        // Toggle the visibility of the Final repositories list
        finalRepositoriesList.style.display = finalRepositoriesList.style.display === 'none' ? 'block' : 'none';
      });

      // Display the specified repositories for Prelim Period
      const prelimRepositoriesList = document.getElementById('prelim-dropdown');
      prelimRepositoriesList.style.display = 'none';

      // Add click event listener to Prelim Period button
      document.getElementById('prelim-period').addEventListener('click', function () {
        // Toggle the visibility of the Prelim repositories list
        prelimRepositoriesList.style.display = prelimRepositoriesList.style.display === 'none' ? 'block' : 'none';
      });

      // Display the specified repositories for Midterm Period
      const midtermRepositoriesList = document.getElementById('midterm-dropdown');
      midtermRepositoriesList.style.display = 'none';

      // Add click event listener to Midterm Period button
      document.getElementById('midterm-period').addEventListener('click', function () {
        // Toggle the visibility of the Midterm repositories list
        midtermRepositoriesList.style.display = midtermRepositoriesList.style.display === 'none' ? 'block' : 'none';
      });
    });
  </script>
</body>

</html>
