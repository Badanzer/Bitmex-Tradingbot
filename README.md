# Bitmex-Tradingbot
The Bot is reading Gmail Signals and opens short or long positions on Bitmex.
You can set Alerts on Tradingview and Tradingview will send you a e-mail if the Alert gets triggert.
(Trade carefully and i don't take any liability for losses. So Please test your settings and the bot with a low quantitiy)

## How to setup the bot?
1. Creat a new Gmail account and enable IMAP and allow less secure apps connecting to your account.
2. Set up your Tradingsignals (Tradingview alerts) or you just can send yourself a e-mail. You also can set the Signal direct in the UI.
3.Fill in the UI (Bitmex API Key, Bitmex secret, Gmail login, Gmail pw, Subject in your e-mails for short and long positions, your quantity (Pleas use a low quantity for testing like 1) of the trades and also the leverage.
4. Start the bot and you are good to go. (Please keep in mind that trading on Bitmex is very risky)

## How does the bot work?
1. The Bot will check your Gmail acc and after he found the right Signal he will open a position with the set quantity and leverage.
2. He keeps checking your Trade and for new Signals.
3. If your Trade goes below -20% gains the trade will be closed and the bot waits for the next Signal.
4. If your Trade goes above 18% gains he will set a Stoploss at Breakeven.
5. If your Trade goes above 30% the bot will use a take profit method. The first take Profit point is at 10% and he will get higher when your gains is also rising.
6. When the bot get a new Signal through your Gmail he will close the open trade and open another one in the opposite direction.

# Here you can see the UI 
![UI](https://user-images.githubusercontent.com/42267648/56431383-c84dc800-62c9-11e9-83dd-dd7a4d21591d.JPG)
