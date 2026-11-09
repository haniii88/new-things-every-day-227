function dailyLog227() {
  const feedback = [
    "positive",
    "positive",
    "neutral",
    "negative",
    "positive",
    "neutral",
    "positive",
    "negative"
  ];

  const total = feedback.length;

  const positive = feedback.filter(item => item === "positive").length;
  const neutral = feedback.filter(item => item === "neutral").length;
  const negative = feedback.filter(item => item === "negative").length;

  console.log("Daily Feedback Report");
  console.log("---------------------");
  console.log(`Total Responses: ${total}`);
  console.log(`Positive: ${(positive / total * 100).toFixed(1)}%`);
  console.log(`Neutral: ${(neutral / total * 100).toFixed(1)}%`);
  console.log(`Negative: ${(negative / total * 100).toFixed(1)}%`);
}

dailyLog227();
