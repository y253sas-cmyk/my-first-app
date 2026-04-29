
const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("CV Builder API is live 🚀");
});

const PORT = process.env.PORT || 10000;

const server = app.listen(PORT, "0.0.0.0", () => {
  console.log("Server running on port " + PORT);
});

server.on("error", (err) => {
  console.error("Server error:", err);
});
