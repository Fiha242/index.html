# index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Pawmodoro</title>
  <link rel="stylesheet" href="style.css"/>
</head>
<body>
  <!-- ✅ Auth Section for Login/Register -->
  <section id="auth-section">
    <h2>🔐 Login or Register</h2>
    <form id="auth-form">
      <input type="email" id="email" placeholder="Email" required />
      <input type="password" id="password" placeholder="Password" required />
      <button type="submit" id="login-btn">Login</button>
      <button type="button" id="register-btn">Register</button>
    </form>
    <p id="auth-error" class="error-text"></p>
  </section>


  <!-- ✅ Main App Section -->
  <div id="app-section">
    <header>
      <h1>🐾 Pawmodoro</h1>
      <a href="settings.html" class="settings-link">⚙ Settings</a>
    </header>


    <!-- Timer Section -->
    <section class="timer-section">
      <div id="time">25:00</div>
      <div class="buttons">
        <button id="start">Start</button>
        <button id="pause">Pause</button>
        <button id="reset">Reset</button>
      </div>
      <p>Pomodoros Completed: <span id="completed-count">0</span></p>
    </section>


    <!-- To-Do List Section -->
    <section class="todo-section">
      <h2>✅ To-Do Checklist</h2>
      <form id="todo-form">
        <input type="text" id="todo-input" placeholder="Add a task..." required />
        <button type="submit">Add</button>
      </form>
      <p id="task-stats">0/0 tasks completed</p>
      <ul id="todo-list"></ul>
    </section>


    <!-- Pet Section -->
    <section class="pet-section">
      <h2>🎁 Your Virtual Pet</h2>
      <img id="pet-image" src="pet1.png" alt="Pet" />
    </section>


    <!-- ✅ Progress Visualization -->
    <section id="progress-section">
      <h2>📊 Your Progress</h2>
      <p>Streak: <span id="streak-count">0</span> days</p>
      <p>Total Sessions Completed: <span id="total-sessions">0</span></p>
    </section>
  </div>


  <!-- Sound -->
  <audio id="finish-sound" src="finish.mp3" preload="auto"></audio>


  <!-- Script -->
  <script src="script.js"></script>
</body>
</html>



