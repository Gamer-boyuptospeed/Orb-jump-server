const express = require("express");
const app = express();
const PORT = process.env.PORT || 3000;

app.use(express.json());

// test route
app.get("/", (req, res) => {
  res.send("Orb Jump Server is running ✅");
});

// placeholder leaderboard route
app.get("/get-leaderboard", (req, res) => {
  res.json([
    { name: "AAA", score: 123 },
    { name: "BBB", score: 99 }
  ]);
});

// placeholder submit route
app.post("/submit-score", (req, res) => {
  const { name, score } = req.body;
  console.log(`Received score: ${name} - ${score}`);
  res.json({ status: "ok" });
});

app.listen(PORT, () => {
  console.log(`Server running on port ${PORT}`);
});
