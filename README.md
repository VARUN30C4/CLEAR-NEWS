import React, { useEffect, useState } from "react";
import axios from "axios";

function App() {
  const [articles, setArticles] = useState([]);

  useEffect(() => {
    // Example: Use a public news API
    axios.get("https://newsapi.org/v2/top-headlines?country=us&apiKey=YOUR_API_KEY")
      .then(response => setArticles(response.data.articles))
      .catch(error => console.error(error));
  }, []);

  return (
    <div>
      <h1>Latest News</h1>
      <div>
        {articles.map((article, idx) => (
          <div key={idx} style={{ border: "1px solid #ccc", margin: "10px", padding: "10px" }}>
            <h2>{article.title}</h2>
            <img src={article.urlToImage} alt="" style={{ width: "100%" }} />
            <p>{article.description}</p>
            <a href={article.url} target="_blank" rel="noopener noreferrer">Read more</a>
          </div>
        ))}
      </div>
    </div>
  );
}

export default App;
