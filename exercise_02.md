# Exercise_02
```
import pygame


pygame.init()
speed = [-3,1]#规定出指定图案的速度
    
screen = pygame.display.set_mode((800,800))#绘制一定大小的对话框
pygame.display.set_caption("Moving")#标题定为moving
object = pygame.image.load("D:\Ein.jpg")#导入图片
position = object.get_react()#屏幕响应
while True:
     for event in pygame.event.get():
         if event.type==pygame.QUIT:
             pygame.quit() 
             break
             exit() #可以正常退出
position = position.move(speed)
screen.bilt(object,position)
pygame.display.flip()
pygame.time.delay(20)
#帧数延时，可以观察到移动
 
```
