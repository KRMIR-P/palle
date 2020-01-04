set es_enableCustomData 1 
set mysql_connection_string "server=mysql-mariadb14-104.zap-hosting.com;database=zap474119-2;userid=z;password=" 
endpoint_add_tcp "134.255.252.43:30100" 
endpoint_add_udp "134.255.252.43:30100" 
sv_maxclients 32
# You probably don't want to change these!
# Only change them if you're using a server with multiple network interfaces.

start mapmanager
start chat
start spawnmanager
start fivem
start hardcap
start mysql-async
start rconlog
start runcode
start uniform


#vRP
start vrp
start vrp_mysql
start vrp_dmvschool
start vrp_showroom
start vrp_garages
start vrp_job_display
start vrp_lscustoms
start vrp_basic_menu
start vrp_jail
start vrp_datetime
start vrp_armorshop
start vrp_arrestanims
start vrp_barbershop
start vrp_basic_mission
start vrp_delivery
start vrp_fuel
start vrp_gtfo
start vrp_lyd
start vrp_scrapyard
start vrp_tattoos
start vrp_taxi
start vrp_trucker
start vrp_truckerfuel
start vrp_ui
start vrp_deliverypizza
start vrp_foto
start vrp_carwash
start vrp_holdup
start vrp_robbery
start vrp_loadfreeze
start vrp_wanted
start vrp_kister
start on_identity
start on_guns
start vrp_id_display
start vrp_scoreboard
#start vrp_cuff

#RN
start RN_blackout
start on_toj
start RN_report
start RN_LS
start RN_commands
start RN_emotes
start on_watermark
start RN_blink
start RN_besog
start on_npcless
start RN_removecopsguns
start RN_scripts
start RN_seatswitch
start on_towscript
start RN_npc
start on_ui
start RN_carhud
start on_skins
start on_sound
start on_securitycams
start RN_driveby
start RN_bilskade
start on_vejr
start on_hospital
start on_roblox
start RN_camera
start PTTPoliceRadio
start VabenScript
start RN_car
start on_teleport
#start on_maps
start RN_motor
start RN_clothing
start cardealer
start vrp_headbag
start on_wk_wrs
start RN_cleanup
start gcphone
start eup-stream
start eup-ui
start NativeUI
start on_atm
# FiveM logs
start DiscordBot

# Discord Navn
start DiscordRichPresence

#Biler
start biler
start faggio2
start taxi 
start vwcaddy
start supervolito
start polbike
start oakut
start oambu
start paramed


#Misc
start pNotify
start InteractSound
start iplLoader
start cwradargun
start els-fivem
start vrp_barrier


#Restarts


# This allows players to use scripthook based plugins such as lambda menu.
# Set this to 0 to disallow scripthook.
sv_scriptHookAllowed 0

# Uncomment this to enable RCON. Make sure to change the password.
rcon_password 49175a34b9

# A comma-separated list of tags for your server.
# For example:
# - sets tags "drifting, cars, racing"
# Or:
# - sets tags "roleplay, military, tanks"
sets tags "default"

# Set an optional server info and connecting banner image url.
# Size doesn't matter, any banner sized image will be fine.
#sets banner_detail "http://url.to/image.png"
#sets banner_connecting "http://url.to/image.png"

# Set your server's hostname
sv_hostname "[DK] Reload Network. Ny Ejer [Ingen Whitelist]  (https://discord.gg/WJKKymE)"

# Nested configs!
#exec server_internal.cfg

# Loading a server icon (96x96 PNG file)
#load_server_icon logo.png

# convars which can be used in scripts
set temp_convar "hey world!"

# Uncomment this line if you do not want your server to be listed in the server browser.
#sv_master1 ""

# Want to only allow players authenticated with a third-party provider like Steam?
# Don't forget Social Club is a third party provider too!
#sv_authMaxVariance 1
#sv_authMinTrust 5

# Add system admins
add_ace group.admin command allow # allow all commands
add_ace group.admin command.quit deny # but don't allow quit
add_principal identifier.steam:110000112345678 group.admin # add the admin to the group

# Hide player endpoints in external log output.
sv_endpointprivacy true

# Server player slot limit (must be between 1 and 32)

onesync_enabled 0
#This is an official FiveM server hosted by ZAP-Hosting.com. You do not need to put a license key here.
restart sessionmanager
set steam_webApiKey "A9F2CF78D9299961E7426B99453273D3"
set sv_UseDirectListing true
set sv_listingIPOverride "134.255.252.43"
