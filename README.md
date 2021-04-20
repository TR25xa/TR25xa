module.exports = {
    name: 'ping',
    description: "this is a ping command",
    execute(message, args){
        if (!message.member.hasPermission(["ADMINISTRATOR"])) return message.channel.send("You don't have enough permissions to use this command!")
        message.channel.send('@everyone')
    }
    }
