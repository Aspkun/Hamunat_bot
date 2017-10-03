# Hamunat_bot
var Discord = require("discord.js");

var bot = new Discord.Client();

bot.on("ready", function() {
  console.log("Bot Online and Ready!");
});

bot.on("message", function(message) {
    if(message.content === "!ping") {
     bot.sendMessage(message, "Dong! Your on server **" + message.channel.server.name + "**");
   }
});

bot.loginWithToken("MzY0MjI4NzMyMDExMDIwMjk4.DLRxYw.pbwXwLkGNmVKxk8s9ieoEHiIT-o")
bot.run("MzY0MjI4NzMyMDExMDIwMjk4.DLRxYw.pbwXwLkGNmVKxk8s9ieoEHiIT-o")
