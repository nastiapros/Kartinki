import pygame
from pygame.draw import polygon, circle

pygame.init()

FPS=30
screen = pygame.display.set_mode((600, 400))

# Фон
pygame.draw.rect(screen, (15, 250, 255), (0, 0, 600, 200))
pygame.draw.rect(screen, (0, 160, 0), (0, 200, 600, 200))
# Дом
pygame.draw.rect(screen, (150, 75, 0), (70, 150, 150, 120))
pygame.draw.rect(screen, (95, 158, 160), (110, 180, 70, 50))
polygon(screen, (178, 34, 34), [(150, 70), (270, 150), (30, 150)])

# Дерево
pygame.draw.rect(screen, (101, 50, 33), (400, 170, 20, 100))
circle(screen, (1, 50, 32), (410, 90), 30)
circle(screen, (0, 0, 0), (410, 90), 30, 2)
circle(screen, (1, 50, 32), (430, 116), 30)
circle(screen, (0, 0, 0), (430, 116), 30, 2)
circle(screen, (1, 50, 32), (385, 116), 30)
circle(screen, (0, 0, 0), (385, 116), 30, 2)
circle(screen, (1, 50, 32), (410, 140), 30)
circle(screen, (0, 0, 0), (410, 140), 30, 2)
circle(screen, (1, 50, 32), (385, 165), 30)
circle(screen, (0, 0, 0), (385, 165), 30, 2)
circle(screen, (1, 50, 32), (430, 165), 30)
circle(screen, (0, 0, 0), (430, 165), 30, 2)
# Облако
circle(screen, (255, 255, 255), (250, 30), 20)
circle(screen, (0, 0, 0), (250, 30), 20, 1)
circle(screen, (255, 255, 255), (270, 40), 20)
circle(screen, (0, 0, 0), (270, 40), 20, 1)
circle(screen, (255, 255, 255), (290, 40), 20)
circle(screen, (0, 0, 0), (290, 40), 20, 1)
circle(screen, (255, 255, 255), (310, 30), 20)
circle(screen, (0, 0, 0), (310, 30), 20, 1)
circle(screen, (255, 255, 255), (270, 20), 20)
circle(screen, (0, 0, 0), (270, 20), 20, 1)
circle(screen, (255, 255, 255), (290, 20), 20)
circle(screen, (0, 0, 0), (290, 20), 20, 1)
# Солнце
circle(screen, (245, 221, 10), (550, 40), 30)
pygame.draw.line(screen,(245, 221, 10),(550,40),(500,30), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(600,30), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(500,50), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(600,50), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(505,70), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(595,70), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(515,90), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(585,90), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(550,95), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(550,0), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(595,5), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(570,0), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(505,5), 10)
pygame.draw.line(screen,(245, 221, 10),(550,40),(530,0), 10)

pygame.display.update()
clock = pygame.time.Clock()
finished = False

while not finished:
    clock.tick(FPS)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True

pygame.quit()