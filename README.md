# exportjson_colmod

```exportjson_colmod.js``` is a modified version of [pamelefox's](https://github.com/pamelafox) JS tool [```exportjson.js```](https://gist.githubusercontent.com/pamelafox/1878143/raw/6c23f71231ce1fa09be2d515f317ffe70e4b19aa/exportjson.js), which now allows users to convert Google Sheets tables to JSON format by rows OR columns.
<br><br>
As I began to delve into the world of game localization with my own project, I wanted to set up a string database in a spreadsheets tool rather than manually entering key:value pairs into a json file. That's when I stumbled across [this tutorial](https://thenewstack.io/how-to-convert-google-spreadsheet-to-json-formatted-text/) which led me to pamelafox's script. However, it only allowed users to setup key:value pairs horizontally along rows, which didn't sit right with my OCD. So here I bring to you, ```exportjson_colmod.js``` (name is a WIP).

## Setup

**Note: You can follow along below, or just use the tutorial I used [here](https://thenewstack.io/how-to-convert-google-spreadsheet-to-json-formatted-text/) and replace pamelafox's script with mine.**

1. Create a new Spreadsheet, entering keys into Column A and values into Column B.<br><br>![exportjsonrepo_ss01](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/f6eb4cc3-559c-4a88-9f68-07c0f6d4d5c8)<br><br>
2. Go to ```View > Freeze > 1 column``` to freeze the first column. This column will be read as keys by the Apps Script.<br><br>![exportjsonrepo_ss02](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/9f7f91e7-18a8-450c-aa78-307749e9d20b)<br><br>![exportjsonrepo_ss03](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/a09e0e36-9723-440f-9431-26142f7d3818)<br><br>
3. Next, go to ```Extensions > Apps Scripts``` which will open a new Script. Go ahead and rename it whatever you'd like and copy and paste the contents of [```exportjson_colmod.js```]() into it. Then click the save icon.<br><br>![exportjsonrepo_ss05](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/d5ea73ae-2197-4293-9870-a561c02196d0)<br><br>![exportjsonrepo_ss06](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/f6658b4f-b51e-48c2-b389-8a99314929d5)<br><br>
4. Now click Run and a popup will...well, pop-up. Click ```Review permissions > Advanced > Accept``` to give the script run privileges. It will then execute and should return 2 messages in the console.<br><br>![exportjsonrepo_ss07](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/2f5e94a1-96d0-471d-9f7b-bf8f71b8a390)<br><br>![exportjsonrepo_ss08](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/e37ade84-d183-492e-984e-8943cb583998)<br><br>
5. Go back to your spreadsheet and a new tab should appear called ```Export JSON```. Click ```Export JSON > Export JSON for this sheet``` and a new popup should appear with the converted code!<br><br>![exportjsonrepo_ss09](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/18cbe285-d069-4dc8-9fe2-a13997e6fa57)<br><br>![exportjsonrepo_ss10](https://github.com/Cisc0-gif/JSONdb-Tools/assets/53851069/61bce15c-6a9e-4c92-b2c5-15e00a619a0c)

**ALLL CREDITS GO TO [Pamela Fox](https://github.com/pamelafox) AND HER GOOGLE SHEETS WIZARDRY!**
