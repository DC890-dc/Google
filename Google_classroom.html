<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Friends Chat</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet">
</head>

<body class="bg-dark text-white">

  <div class="container-fluid text-center bg-warning text-dark p-2 shadow">
    <h1>Friends Messaging System</h1>
    <p>Identity enforced. Chaos reduced.</p>
  </div>

  <!-- CHAT FORM -->
  <div class="container bg-secondary p-3 mt-4 w-50 rounded">
    <form id="chatForm">

      <div class="mb-3">
        <label class="form-label">Who are you?</label>
        <select class="form-select" id="sender">
          <option value="">Select your name</option>
          <option>Dev</option>
          <option>Alex</option>
          <option>Sam</option>
          <option>Jordan</option>
        </select>
      </div>

      <div class="mb-3">
        <label class="form-label">Your PIN</label>
        <input type="password" class="form-control" id="pin" placeholder="Only you know this">
      </div>

      <div class="mb-3">
        <label class="form-label">Message</label>
        <input type="text" class="form-control" id="message" placeholder="Type something sane">
      </div>

      <button type="submit" class="btn btn-warning w-100">Send</button>
    </form>
  </div>

  <!-- CHAT DISPLAY -->
  <div class="container bg-light text-dark mt-4 w-50 rounded p-3">
    <h5 class="text-center">Chat</h5>
    <div id="chatBox" style="max-height: 300px; overflow-y: auto;"></div>
  </div>

  <!-- SCRIPT -->
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      const chatForm = document.getElementById("chatForm");
      const chatBox = document.getElementById("chatBox");

      // 🔐 User → PIN mapping
      const users = {
        Dev: "1111",
        Alex: "2222",
        Sam: "3333",
        Jordan: "4444"
      };

      function loadMessages() {
        const messages = JSON.parse(localStorage.getItem("chatMessages")) || [];
        chatBox.innerHTML = "";

        messages.forEach(msg => {
          const div = document.createElement("div");
          div.classList.add("mb-2");
          div.innerHTML = `
            <strong>${msg.sender}</strong>: ${msg.text}
            <span class="text-muted small">(${msg.time})</span>
          `;
          chatBox.appendChild(div);
        });

        chatBox.scrollTop = chatBox.scrollHeight;
      }

      chatForm.addEventListener("submit", e => {
        e.preventDefault();

        const sender = document.getElementById("sender").value;
        const pin = document.getElementById("pin").value;
        const text = document.getElementById("message").value.trim();

        if (!sender || !pin || !text) {
          alert("Name, PIN, and message required.");
          return;
        }

        if (users[sender] !== pin) {
          alert("Wrong PIN. Impersonation denied.");
          return;
        }

        const messages = JSON.parse(localStorage.getItem("chatMessages")) || [];

        messages.push({
          sender,
          text,
          time: new Date().toLocaleTimeString()
        });

        localStorage.setItem("chatMessages", JSON.stringify(messages));
        chatForm.reset();
        loadMessages();
      });

      loadMessages();
    });
  </script>

</body>
</html>
