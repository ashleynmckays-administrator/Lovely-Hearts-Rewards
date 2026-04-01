# Lovely-Hearts-Rewards
A rewards program for collecting hearts that convert your steps into $Rewards
git clone https://github.com/ashleynmckays-administrator/Lovely-Hearts-Rewards.git
cd Lovely-Hearts-Rewards
npm init -y
npm install const express = require('express');
const app express = express();

app.use(express.json());

app.get('/', (req, res) => {
    res.send('Lovely Hearts Rewards Backend!');
});

app.listen(3000, () => console.log('Server is running on port 3000'));



