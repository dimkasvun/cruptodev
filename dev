async function fetchBitcoinPrice() {
    try {
        const response = await fetch('https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=usd');
        if (!response.ok) {
            throw new Error(`HTTP error! Status: ${response.status}`);
        }
        const data = await response.json();
        console.log(`Bitcoin Price: $${data.bitcoin.usd}`);
    } catch (error) {
        console.error('Error fetching data:', error);
    }
}

fetchBitcoinPrice();
