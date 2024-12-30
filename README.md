import speech_recognition as sr  
import pyglet  
import os  
import time  
import webbrowser  
from tqdm import tqdm  
import pyttsx3

engine = pyttsx3.init()

print('запуск N.E.Y.R.O')  
print('Loading...')  
for _ in tqdm(range(10000000), colour="green"):  
    pass  # Используем pass, чтобы избежать ошибок при пустом цикле  

# Воспроизводим звуковые файлы  
nus = pyglet.resource.media("2.wav")  
nus.play()  
time.sleep(2)  
nus = pyglet.resource.media("да сер.wav")  
nus.play()  

# Настройка распознавателя  
recognizer = sr.Recognizer()  
recognizer.pause_threshold = 1

def thenkyou():
    nus = pyglet.resource.media("к вашим устугам сер .wav")  
    nus.play()  



def listen_command():  
    """Обработчик команд с микрофона."""  
    try:  
        with sr.Microphone() as mic:  
            print('N.E.Y.R.O:')  
            recognizer.adjust_for_ambient_noise(mic, duration=1)  
            audio = recognizer.listen(mic)  
            query = recognizer.recognize_google(audio, language='ru-RU').lower()  
            return query  
    except sr.UnknownValueError:  
        return 'Damn... команда не ясна'  
    except Exception as e:  
        print(f"Ошибка: {e}")  
        return ""  

def explorer():
    os.system('explorer.exe')
    
    nus = pyglet.resource.media("есть.wav")  
    nus.play()  

def AI():

    nus = pyglet.resource.media("web.wav")  
    nus.play()

    os.startfile('C:/py/opencv/opencv.py')

def yandex():
    url = 'https://ya.ru'
    webbrowser.open_new_tab(url)
    
    nus = pyglet.resource.media("есть.wav")  
    nus.play() 

def camera():
    os.startfile(r'C:/2/Camera.lnk')


def IDE():
    
    nus = pyglet.resource.media("web.wav")  
    nus.play()

    os.startfile(r'C:/Program Files/Sublime Text/sublime_text.exe')
    
def voice():  
    os.startfile(r'C:/Program Files/Audacity/Audacity.exe')  
    
    nus = pyglet.resource.media("есть.wav")  
    nus.play()


def terminal():  
    os.startfile(r'C:/Users/user/Documents/1/Терминал.lnk')  
    
    nus = pyglet.resource.media("есть.wav")  
    nus.play()


def photoshop():  
    os.startfile(r'C:/Program Files/Adobe/Adobe Photoshop CC 2019/Photoshop.exe')  # Исправленный путь к Photoshop  
    
    nus = pyglet.resource.media("web.wav")  
    nus.play()

def vois():
    engine.say('голос был изменён')
    engine.runAndWait()

def vois2():
    engine.say("не согласен с вами")
    engine.runAndWait()

def vois3():
    engine.say("в аудио драйверах есть ошибка ")
    engine.runAndWait()


def vois4():
    engine.say('жду вашей каманды')
    engine.runAndWait()


def blender():  
    os.startfile(r'C:/Program Files/Blender Foundation/Blender 4.3/blender-launcher.exe')  
    
    nus = pyglet.resource.media("есть.wav")  
    nus.play()

def drift():
    url = 'https://youtu.be/kyzIQKuSqBs?si=eB5pAEILz7D79Bp1'  
    webbrowser.open_new_tab(url)  

    
    nus = pyglet.resource.media("есть.wav")  
    nus.play()

def proceshacker():
    os.startfile(r'C:/Users/user/Desktop/programms/ProcessHacker.exe')

    
    nus = pyglet.resource.media("есть.wav")  
    nus.play()


def montaj():  
   
    nus = pyglet.resource.media("web.wav")  
    nus.play()


    os.startfile(r'C:/Program Files/Shotcut/shotcut.exe')  
    
def chst():
    os.startfile('C:/Users/user/Documents/1/WhatsApp.lnk')


    nus = pyglet.resource.media("есть.wav")  
    nus.play()

def protocol():

    nus = pyglet.resource.media("есть.wav")  
    nus.play()

    nus = pyglet.resource.media("protocol.wav")  
    nus.play()
    
    os.startfile(r'C:/py/N.E.Y.R.O/music.mp3')

def word():
    os.startfile(r'C:/Program Files/Microsoft Office/Office16/WINWORD.EXE')  # Microsoft Word  


def time():
    os.startfile(r'C:/py/main/tim.exe')
    
    nus = pyglet.resource.media("web.wav")  
    nus.play()

def create_task():  
    """Создание задачи в списке дел."""  
    print('Что добавить в список дел?')  
    query = listen_command()  
    with open('todo-list.txt', 'a') as file:  
        file.write(f'! {query}\n')  
    return f'Задача {query} добавлена в todo-list!'
    
    nus = pyglet.resource.media("есть.wav")  
    nus.play()  

def youtube():  
    url = 'https://youtube.com/@tonibrozz?si=jNleOJMPOkz5VNVM'  
    webbrowser.open_new_tab(url)  
    
    nus = pyglet.resource.media("web.wav")  
    nus.play()

def IT():
    url = 'https://youtube.com/@howdyhonet?si=8T7JJzCPQIdXSSVGM'  
    webbrowser.open_new_tab(url)  
    
    nus = pyglet.resource.media("web.wav")  
    nus.play()


def lox():
    nus = pyglet.resource.media("other.wav")  
    nus.play()

def tmt():
    nus = pyglet.resource.media("да сер.wav")  
    nus.play()

def youtube1():  
    url = 'https://youtube.com'  
    webbrowser.open_new_tab(url)  
    
    nus = pyglet.resource.media("web.wav")  
    nus.play()


def поиск():  
    os.startfile(r'C:/Program Files/Everything/Everything.exe')  
    nus = pyglet.resource.media("есть.wav")  
    nus.play()

def пятница():
    engine.say('да сер')
    engine.runAndWait()

def base():
    engine.say('пробиваю по базам даных')
    name = input('Name:')
    engine.say(f'пол женский имя {name} возраст 15 лет зациклина на падлизывание учитилей не люьимый придмет математика а точнейе учителница 158 школы псевдоним Saliga Aliguseynovna')
    engine.runAndWait()



def music():  
    """Воспроизведение музыки."""  
    os.startfile(r'C:/py/N.E.Y.R.O/music.mp3') 
    nus = pyglet.resource.media("есть.wav")  
    nus.play() 

def films():
    
    nus = pyglet.resource.media("web.wav")  
    nus.play()

    url = 'https://kinogo-films.biz/43027-zheleznyj-chelovek-3.html'  
    webbrowser.open_new_tab(url)  
    
    nus = pyglet.resource.media("protocol.wav")  
    nus.play()
    


def google():  
    """Открыть Google Chrome."""  
    os.startfile(r'C:/Program Files/Google/Chrome/Application/chrome.exe')  
    nus = pyglet.resource.media("web.wav")  
    nus.play()

def greeting():  
    """Функция приветствия."""  
    print('да сер') 


def shutdown():  
    os.system("shutdown -s -t 0")  
    nus = pyglet.resource.media("есть.wav")  
    nus.play()

def shutdown2():  
    os.system("shutdown -h")  
    nus = pyglet.resource.media("есть.wav")  
    nus.play()

def friday():  
    nus = pyglet.resource.media("да сер.wav")  
    nus.play()  

def main():  
    while True:  # Бесконечный цикл  
        query = listen_command()  
        
        if query == "":  
            continue  # Пропустить пустые команды  

        if query == "ты тут":  
            greeting()  

        elif query == 'блендер':  
            blender()  
        
        elif query == 'чат':
            chst()

        elif query == 'лео чат':
            chst()

        elif query == 'запустить чат':
            chst()
       
        elif query == 'запусти чат':
            chst()


        elif query == 'хауди хо':
            IT()

        elif query == 'посмотрим фильм':
            films()


        elif query == 'фильм':
            films()

        elif query == 'протокол фильм':
            films()


        elif query == 'нейро фильм':
            films()


        elif query == 'запустить блендер':  
            blender()  

        elif query == 'открой блендер':  
            blender()  
        
        elif query == 'изменить голос':
            vois()

        elif query == 'протокол отдых':
            protocol()

        elif query == 'протокол отдыха':
            protocol()

        elif query == 'яндекс':
            yandex()

        elif query == 'камера':
            camera()

        elif query  == 'что делаеш':
            vois4()

        elif query == 'чем занеть':
            vois4()

        elif query == 'протокол дрифт':
            drift()

        elif query == 'тб':
            youtube1()

        elif query == 'нейро тб':
            youtube1()


        elif query == 'нейро открой тб':
            youtube1()

        elif query == 'ты дурак':
            lox()

        elif query == 'проверка':
            proceshacker()

        elif query == 'где ошибка':
            vois3()

        elif query == 'открыть блендер':  
            blender()  
        
        elif query == 'диктофон':  
            voice()  
        
        elif query == 'таймер':
            time()

        elif query == 'монтаж':  
            montaj()  
        
        elif query == 'документы':
            word()  
        
        elif query == 'запустить монтаж':  
            montaj()

        elif query == 'спасибо':
            thenkyou()

        elif query == 'файлы':
            explorer()

        elif query == 'баг':
            lox()

        elif query == 'глюки':
            lox()

        elif query == 'нейро в коде ошибка':
            lox()


        elif query == 'в коде ошибка':
            lox()


        elif query == 'в есть коде ошибка':
            lox()


        elif query == 'есть ошибка':
            lox()


        elif query == 'открой файлы':
            explorer()

        elif query == 'открыть праводник':
            explorer()

        elif query == 'нейро открой праводник':
            explorer()

        elif query == 'открой монтаж':  
            montaj()  
        
        elif query == 'открыть монтаж':  
            montaj()  

        elif query == 'канал':  
            youtube()            
        
        elif query == 'открой терминал':  
            terminal()  
        
        elif query == 'терминал':  
            terminal()  

        elif query == 'выключи':  
            shutdown()  

        elif query == 'фото':  
            photoshop()  

        elif query == 'открой фото':  
            photoshop()  

        elif query == 'открыть фото':  
            photoshop()  

        elif query == 'открой редактор':  
            IDE()  # Предполагается, что функция IDE() определена  
        
        elif query == 'открыть редактор':  
            IDE()  # Предполагается, что функция IDE() определена  
            
        elif query == 'редактор':  
            IDE()  # Предполагается, что функция IDE() определена  

        elif query == 'поиск':  
            поиск()  
        
        elif query == 'база':
            base()

        elif query == 'открой поиск':  
            поиск()  
        
        elif query == 'открыть поиск':  
            поиск()  

        elif query == 'браузер':  
            google()  

        elif query == 'открой браузер':  
            google()  

        elif query == 'открыть браузер':  
            google()  
        
        elif query == 'запусти оприделение':
            AI()


        elif query == 'запустить определение':
            AI()


        elif query == 'открыть определение':
            AI()


        elif query == 'выключить и запомнить':  
            shutdown2()  

        elif query == 'включить музыку':  
            music()  


        elif query == 'вруби музон':  
            music()  


        elif query == 'музыка':  
            music()  

        elif query == 'нейро музыка':
            music()

        elif query == 'добавить задачу':  
            create_task()

        elif query == 'задача':  
            create_task()

        elif query == 'нейро':  
            friday()  

        elif query == 'выход':  
            print("Выход из программы.")  
            break  # Завершить цикл и выйти из программы  

        elif query == 'закрыть':  
            print("Выход из программы.") 
            nus = pyglet.resource.media("есть.wav")  
            nus.play() 
            break  # Завершить цикл и выйти из программы  

        elif query == 'выход':
            nus = pyglet.resource.media("есть.wav")  
            nus.play()
            exit()


        else:  
            print('каманда не ясна')  

if __name__ == '__main__':  
    main()
