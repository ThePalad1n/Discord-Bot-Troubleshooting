# Discord-Bot-Troubleshooting






#I have one bracket error. Try copy and pasting on VScode.







module.exports = {
    name: 'command',
    description: "Embeds!",
    
    execute(message, args, Discord){
    
    
        const newEmbed = new Discord.MessageEmbed()
        .setColor('#304281')
        .setTitle('Rules')
        .setURL('https://www.google.com')
        .setDescription('This is an embed for the server rules')
        .addFields(
            {name: 'Rule 1', value: 'Do NOT talk about Neurotators.'},
            {name: 'Rule 2', value: 'Understand Rule 1.'},
            {name: 'Rule 3', value: 'Be respectful. See Rule 4.'},
            {name: 'Rule 4', value: 'No slurs or hate speech. See Rule 3.'},
            {name: 'Rule 5', value: 'Discussion should be geared toward science, whether quantum mechanical or sociological.'},
            {name: 'Rule 6', value: 'Have fun!'},
        )
        .setImage('https://www.lead-dbs.org/wp-content/uploads/HarvardOxford-261x300.png'),
        <div>
        .setFooter('Make sure to check out the Rules channel, mkay?')
        </div>
        message.channel.send({embeds: [newEmbed]}
        }
    
}
