## Hi there 👋

<!--
**jsmoothcreativity/jsmoothcreativity** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<h1 align="right">Greetings 👋, I'm Jean Janvier</h1>
<h3 align="right">Dynamic Senior Developer with 7 years of experience in backend development, ERP integrations, and cloud infrastructure management. Currently pursuing a Master’s in Cybersecurity Intelligence, focusing on building secure, scalable, and high-performance systems. Adept at leading cross-functional teams, managing external developers, and transitioning legacy systems into modern architectures. Ready to deliver seamless solutions and drive innovation as a Full Stack Developer.</h3>

<p align="left"> <img src="https://komarev.com/ghpvc/?username=githubusername&label=Profile%20views&color=0e75b6&style=flat" alt="githubusername" /> </p>

<p align="left"> <a href="https://github.com/ryo-ma/github-profile-trophy"><img src="https://github-profile-trophy.vercel.app/?username=githubusername" alt="githubusername" /></a> </p>

<p align="left"> <a href="https://twitter.com/" target="blank"><img src="https://img.shields.io/twitter/follow/?logo=twitter&style=for-the-badge" alt="" /></a> </p>

- 🔭 I’m currently working on **Ticket Marketplace Platform**

- 🌱 I’m currently learning **Cybersecurity**


<div style="padding: 20px; max-width: 400px; margin: 50px auto; background: white; border-radius: 8px; box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1); font-family: Arial, sans-serif; text-align: center;">
    <h1 style="font-size: 24px; margin-bottom: 20px;">Tech Quiz</h1>
    <div id="quiz">
      <p id="question" style="margin-bottom: 20px;">Loading question...</p>
      <div id="answers"></div>
    </div>
    <div id="result" style="margin-top: 20px; font-size: 20px; font-weight: bold;"></div>
    <button id="nextQuestion" style="display:none; margin-top: 20px; padding: 10px 20px; font-size: 16px; border: none; background-color: #007bff; color: white; border-radius: 5px; cursor: pointer;">Try a New Question</button>
  </div>

  <script>
    const questions = [
      {
        question: "Which programming language is used for web development and has a logo featuring a coffee cup?",
        answers: [
          { text: "JavaScript", correct: false },
          { text: "Python", correct: false },
          { text: "Java", correct: true },
          { text: "C++", correct: false }
        ]
      },
      {
        question: "What does CSS stand for?",
        answers: [
          { text: "Cascading Style Sheets", correct: true },
          { text: "Creative Style Sheets", correct: false },
          { text: "Colorful Style Sheets", correct: false },
          { text: "Computer Style Sheets", correct: false }
        ]
      },
      {
        question: "Which of these is a cybersecurity concept?",
        answers: [
          { text: "Phishing", correct: true },
          { text: "Trawling", correct: false },
          { text: "Casting", correct: false },
          { text: "Netting", correct: false }
        ]
      },
      {
        question: "What is the primary purpose of a firewall in cybersecurity?",
        answers: [
          { text: "To filter incoming and outgoing network traffic", correct: true },
          { text: "To cool down overheating systems", correct: false },
          { text: "To block all internet access", correct: false },
          { text: "To store data securely", correct: false }
        ]
      }
    ];

    let currentQuestionIndex = Math.floor(Math.random() * questions.length);
    let askedQuestions = new Set();

    function loadQuestion() {
      const questionElement = document.getElementById('question');
      const answersElement = document.getElementById('answers');
      const resultElement = document.getElementById('result');
      const nextButton = document.getElementById('nextQuestion');

      resultElement.textContent = '';
      nextButton.style.display = 'none';

      const currentQuestion = questions[currentQuestionIndex];
      questionElement.textContent = currentQuestion.question;

      answersElement.innerHTML = '';
      currentQuestion.answers.forEach(answer => {
        const button = document.createElement('button');
        button.textContent = answer.text;
        button.style = "padding: 10px 20px; margin: 10px; font-size: 16px; border: none; background-color: #007bff; color: white; border-radius: 5px; cursor: pointer;";
        button.onmouseover = () => button.style.backgroundColor = '#0056b3';
        button.onmouseout = () => button.style.backgroundColor = '#007bff';
        button.onclick = () => checkAnswer(answer.correct);
        answersElement.appendChild(button);
      });
    }

    function checkAnswer(correct) {
      const result = document.getElementById('result');
      const nextButton = document.getElementById('nextQuestion');

      if (correct) {
        result.textContent = '🎉 Correct!';
        result.style.color = 'green';
        askedQuestions.add(currentQuestionIndex);
        nextButton.style.display = 'inline-block';
        nextButton.onclick = loadNextQuestion;
      } else {
        result.textContent = '❌ Oops! Try again.';
        result.style.color = 'red';
      }
    }

    function loadNextQuestion() {
      if (askedQuestions.size === questions.length) {
        alert('You have answered all questions! Resetting quiz.');
        askedQuestions.clear();
      }

      do {
        currentQuestionIndex = Math.floor(Math.random() * questions.length);
      } while (askedQuestions.has(currentQuestionIndex));

      loadQuestion();
    }

    loadQuestion();
  </script>


<h3 align="left">Connect with me:</h3>
<p align="left">
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://angular.io" target="_blank" rel="noreferrer"> <img src="https://angular.io/assets/images/logos/angular/angular.svg" alt="angular" width="40" height="40"/> </a> <a href="https://aws.amazon.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="aws" width="40" height="40"/> </a> <a href="https://azure.microsoft.com/en-in/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/microsoft_azure/microsoft_azure-icon.svg" alt="azure" width="40" height="40"/> </a> <a href="https://www.gnu.org/software/bash/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/gnu_bash/gnu_bash-icon.svg" alt="bash" width="40" height="40"/> </a> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://canvasjs.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/Hardik0307/Hardik0307/master/assets/canvasjs-charts.svg" alt="canvasjs" width="40" height="40"/> </a> <a href="https://www.chartjs.org" target="_blank" rel="noreferrer"> <img src="https://www.chartjs.org/media/logo-title.svg" alt="chartjs" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cs/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" alt="csharp" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://dotnet.microsoft.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/dot-net/dot-net-original-wordmark.svg" alt="dotnet" width="40" height="40"/> </a> <a href="https://cloud.google.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://graphql.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/graphql/graphql-icon.svg" alt="graphql" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.jenkins.io" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/jenkins/jenkins-icon.svg" alt="jenkins" width="40" height="40"/> </a> <a href="https://kubernetes.io" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/kubernetes/kubernetes-icon.svg" alt="kubernetes" width="40" height="40"/> </a> <a href="https://laravel.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/laravel/laravel-plain-wordmark.svg" alt="laravel" width="40" height="40"/> </a> <a href="https://mariadb.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/mariadb/mariadb-icon.svg" alt="mariadb" width="40" height="40"/> </a> <a href="https://www.microsoft.com/en-us/sql-server" target="_blank" rel="noreferrer"> <img src="https://www.svgrepo.com/show/303229/microsoft-sql-server-logo.svg" alt="mssql" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://www.nginx.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg" alt="nginx" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://www.oracle.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/oracle/oracle-original.svg" alt="oracle" width="40" height="40"/> </a> <a href="https://www.php.net" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/php/php-original.svg" alt="php" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://sass-lang.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sass/sass-original.svg" alt="sass" width="40" height="40"/> </a> <a href="https://spring.io/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/springio/springio-icon.svg" alt="spring" width="40" height="40"/> </a> <a href="https://www.sqlite.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/sqlite/sqlite-icon.svg" alt="sqlite" width="40" height="40"/> </a> <a href="https://www.typescriptlang.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/> </a> <a href="https://dotnet.microsoft.com/apps/xamarin" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/detain/svg-logos/780f25886640cef088af994181646db2f6b1a3f8/svg/xamarin.svg" alt="xamarin" width="40" height="40"/> </a> </p>

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=githubusername&show_icons=true&locale=en&layout=compact" alt="githubusername" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=githubusername&show_icons=true&locale=en" alt="githubusername" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=githubusername&" alt="githubusername" /></p>
