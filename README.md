# personal-crypto-ticker

https://hpssjellis.github.io/personal-crypto-ticker/public/index.html



```

2023 A better site is <a href="https://coincap.io">coincap.io</a> <br>



<input id="showTicker" type="button" value="Recent prices" onclick="getRecentPrices()">

<script>
  async function getRecentPrices() {
    try {
      const url = 'https://api.coincap.io/v2/assets/bitcoin?';
      const response = await fetch(url);
      if (!response.ok) {
        throw new Error('Network response was not ok');
      }
      const data = await response.json();
      console.log(data);
    } catch (error) {
      console.error('An error occurred:', error);
    }
  }
</script>
```
