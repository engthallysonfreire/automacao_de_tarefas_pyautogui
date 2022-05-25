import pyautogui
from time import sleep

#pyautogui.write -> escreve
#pyautogui.click -> clica
#pyautogui.locateOnScreen -> identifica uma imagem na sua tela
#pyautogui.hotkey -> usa atalhos do teclado
#pyautogui.press -> aperta um botão do teclado
#print(pyautogui.KEYBOARD_KEYS) -> comandos do pacote


#abrir o sistema (abrir o navegador - Google Chrome)

pyautogui.PAUSE = 1.5
#apertar a tecla windows do teclado
pyautogui.press('win')
#digitar "chrome" no navegador windows
pyautogui.write("chrome")
#apertar enter
pyautogui.press('enter')
#entrar no LinkedIn
pyautogui.write("linkedin ")
pyautogui.press('enter')
#localizar a imagem -> vai me dar 4 informações: pos x, pos y, larg, alt
x, y, largura, altura = pyautogui.locateOnScreen("busca_google.png")
#clicar no meio da imagem
pyautogui.click(x + largura/2, y + altura/2)
#esperar LinkedIn
while not pyautogui.locateOnScreen('logo_linkedin.png'):
    sleep(1)
    
#publicar no linkedin
x, y, largura, altura = pyautogui.locateOnScreen("publicar.png")
pyautogui.click(x + largura/2, y + altura/2)

#texto
pyautogui.write("""Desenvolvi esta pequena automação em Python utilizando o pacote Pyautogui, que permite executar
tarefas usando nosso teclado e mouse. 
É uma automação simples, apenas como forma de aprendizado. 
Esse pacote é muito incrível, pois, utilizando-o somando a outros, o limite é até onde vai a sua imaginação
para automatizar processos. Inclusive, este texto que estou digitando e publicando aqui, no LinkedIn, está sendo feito de maneira autônoma.
O código está acessando links, pastas e arquivos.
(vídeo abaixo)""")
