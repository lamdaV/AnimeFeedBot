# AnimeFeedBot
A simple discord bot to notify your channels of upcoming anime
showings.

## Purpose
I wrote this bot to familiarize myself with the discord developer tools.

## Commands
**Note:** All commands are prefixed with `->`.

- `-> help` responds with a list of commands available.
- `-> anime-today` responds with a listing of anime showings of the current date.
- `-> update` sets the channel to be updated regularly every 24 hour interval
- `-> praise-the-sun` responds with `\[T]/ \[T]/ \[T]/`

## External Dependencies
- [monthly.moe](https://www.monthly.moe/)

## Setup
1. Clone the repository
```
git clone https://github.com/lamdaV/AnimeFeedBot.git
```

2. Create a logs directory
```
cd AnimeFeedBot
mkdir logs
touch logs/bot.log
```

3. Install dependencies
```
npm install
// or
yarn install
```

4. Create a `.env` file with your token
```
echo "DISCORD_TOKEN=YOUR_DISCORD_TOKEN" > .env
```

5. Start the bot.
```
npm run start
// or
yarn start
```

## Using pm2
1. Install pm2 globally
```
npm install -g pm2
```

2. Start bot with pm2
```
cd AnimeFeedBot
pm2 start src/bot.js --name AnimeFeedBot
```

## Development
Run through the [Setup](#setup) once. Run
```
npm run dev
// or
yarn dev
```
