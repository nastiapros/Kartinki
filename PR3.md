import pygame
from pygame.draw import polygon, circle

pygame.init()

FPS=30
screen = pygame.display.set_mode((1000, 600))

# Фон
pygame.draw.rect(screen, (15, 250, 255), (0, 0, 1000, 300))
pygame.draw.rect(screen, (0, 160, 0), (0, 300, 1000, 300))

# Дома
pygame.draw.rect(screen, (150, 75, 0), (100, 330, 200, 180))
pygame.draw.rect(screen, (95, 158, 160), (150, 380, 100, 80))
polygon(screen, (178, 34, 34), [(210, 220), (340, 330), (60, 330)])

pygame.draw.rect(screen, (150, 75, 0), (570, 320, 160, 140))
pygame.draw.rect(screen, (95, 158, 160), (610, 360, 80, 60))
polygon(screen, (178, 34, 34), [(650, 260), (540, 320), (760, 320)])

# Деревья
pygame.draw.rect(screen, (101, 50, 33), (420, 350, 30, 150))
circle(screen, (1, 50, 32), (430, 230), 40)
circle(screen, (0, 0, 0), (430, 230), 40, 2)
circle(screen, (1, 50, 32), (380, 270), 40)
circle(screen, (0, 0, 0), (380, 270), 40, 2)
circle(screen, (1, 50, 32), (470, 270), 40)
circle(screen, (0, 0, 0), (470, 270), 40, 2)
circle(screen, (1, 50, 32), (430, 290), 40)
circle(screen, (0, 0, 0), (430, 290), 40, 2)
circle(screen, (1, 50, 32), (400, 330), 40)
circle(screen, (0, 0, 0), (400, 330), 40, 2)
circle(screen, (1, 50, 32), (460, 330), 40)
circle(screen, (0, 0, 0), (460, 330), 40, 2)

pygame.draw.rect(screen, (101, 50, 33), (845, 315, 20, 100))
circle(screen, (1, 50, 32), (855, 220), 30)
circle(screen, (0, 0, 0), (855, 220), 30, 2)
circle(screen, (1, 50, 32), (820, 250), 30)
circle(screen, (0, 0, 0), (820, 250), 30, 2)
circle(screen, (1, 50, 32), (890, 250), 30)
circle(screen, (0, 0, 0), (890, 250), 30, 2)
circle(screen, (1, 50, 32), (855, 270), 30)
circle(screen, (0, 0, 0), (855, 270), 30, 2)
circle(screen, (1, 50, 32), (830, 300), 30)
circle(screen, (0, 0, 0), (830, 300), 30, 2)
circle(screen, (1, 50, 32), (880, 300), 30)
circle(screen, (0, 0, 0), (880, 300), 30, 2)

# Облака
circle(screen, (255, 255, 255), (220, 100), 30)
circle(screen, (0, 0, 0), (220, 100), 30, 1)
circle(screen, (255, 255, 255), (250, 120), 30)
circle(screen, (0, 0, 0), (250, 120), 30, 1)
circle(screen, (255, 255, 255), (290, 120), 30)
circle(screen, (0, 0, 0), (290, 120), 30, 1)
circle(screen, (255, 255, 255), (320, 100), 30)
circle(screen, (0, 0, 0), (320, 100), 30, 1)
circle(screen, (255, 255, 255), (250, 80), 30)
circle(screen, (0, 0, 0), (250, 80), 30, 1)
circle(screen, (255, 255, 255), (290, 80), 30)
circle(screen, (0, 0, 0), (290, 80), 30, 1)

circle(screen, (255, 255, 255), (500,150), 20)
circle(screen, (0, 0, 0), (500, 150), 20, 1)
circle(screen, (255, 255, 255), (520, 160), 20)
circle(screen, (0, 0, 0), (520, 160), 20, 1)
circle(screen, (255, 255, 255), (550, 160), 20)
circle(screen, (0, 0, 0), (550, 160), 20, 1)
circle(screen, (255, 255, 255), (570, 150), 20)
circle(screen, (0, 0, 0), (570, 150), 20, 1)
circle(screen, (255, 255, 255), (520, 140), 20)
circle(screen, (0, 0, 0), (520, 140), 20, 1)
circle(screen, (255, 255, 255), (550, 140), 20)
circle(screen, (0, 0, 0), (550, 140), 20, 1)

circle(screen, (255, 255, 255), (750, 120), 30)
circle(screen, (0, 0, 0), (750, 120), 30, 1)
circle(screen, (255, 255, 255), (780, 140), 30)
circle(screen, (0, 0, 0), (780, 140), 30, 1)
circle(screen, (255, 255, 255), (820, 140), 30)
circle(screen, (0, 0, 0), (820, 140), 30, 1)
circle(screen, (255, 255, 255), (850, 120), 30)
circle(screen, (0, 0, 0), (850, 120), 30, 1)
circle(screen, (255, 255, 255), (780, 100), 30)
circle(screen, (0, 0, 0), (780, 100), 30, 1)
circle(screen, (255, 255, 255), (820, 100), 30)
circle(screen, (0, 0, 0), (820, 100), 30, 1)

# Солнце
circle(screen, (245, 221, 10), (60, 50), 30)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(10,30), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(110,30), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(10,50), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(110,50), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(15,70), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(105,70), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(25,95), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(95,95), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(60,100), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(60,0), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(105,5), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(80,0), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(15,5), 10)
pygame.draw.line(screen,(245, 221, 10),(60, 50),(40,0), 10)

pygame.display.update()
clock = pygame.time.Clock()
finished = False

while not finished:
    clock.tick(FPS)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True

pygame.quit()