import nextcord
from nextcord.ext import commands
from nextcord.ui import View, Button
import config

bot = commands.Bot(help_command=None)

class VerifyButton(View):
    def __init__(self):
        super().__init__()
        self.value = None

    @nextcord.ui.button(label="Verify", style=nextcord.ButtonStyle.green, emoji="✅")
    async def button1(self, button: Button, interaction: nextcord.Interaction):
        user = interaction.user
        guild = interaction.guild
        role = guild.get_role(config.roleid)  # Replace config.roleid with the actual role ID
        await interaction.response.send_message("Complete", ephemeral=True)
        if role:
            await user.add_roles(role)
        
@bot.slash_command(description="Verify", guild_ids=[config.guild_id])
async def setup(interaction: nextcord.Interaction):
    embed = nextcord.Embed(title="💥 | BOT VERIFY", description="❗ กดปุ่มด้านล่างเพื่อยืนยันตัวตน", color=0xe62063)
    embed.set_image(url="https://cdn.discordapp.com/attachments/1132314482203430942/1136117202827878410/standard.gif")    
    view = VerifyButton()
    
    await interaction.send('สำเร็จ', ephemeral=True)
    await interaction.send(embed=embed, view=view)
    await view.wait()

@bot.event
async def on_ready():
    print(f'BOT NAME : {bot.user}')
    await bot.change_presence(activity=nextcord.Streaming(name=" ",url="https://www.twitch.tv/BIT NAI SON LUK KHRAI"))

bot.run(config.token)
