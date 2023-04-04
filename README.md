# Opensource-chat-gpt-code
html code for a chatgpt based websote
  
  Use this snippet for your site: <!DOCTYPE html>
<html>
  <head>
    <title>Chatbot powered by ChatGPT</title>
    <script src="https://cdn.jsdelivr.net/npm/@openai/chat-api@0.3.1/dist/index.js"></script>
  </head>
  <body>
    <h1>Chatbot powered by ChatGPT</h1>
    <div id="chatbot-container"></div>
    <script>
      const chatbot = new window.ChatApi({
        publicKey: "8585856434",
        engine: "davinci",
        prompt: "Hi, how can I assist you today?",
      });
      chatbot.create({
        container: document.getElementById("chatbot-container"),
        onComplete: (chatHistory) => {
          console.log(chatHistory);
        },
      });
    </script>
  </body>
</html>
