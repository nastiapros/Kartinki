import pygame
from pygame.draw import polygon, circle

pygame.init()

FPS=30
screen = pygame.display.set_mode((800, 600))

pygame.draw.rect(screen, (186, 210, 188), (0, 0, 800, 600))
circle(screen, (255, 240, 3), (400, 300), 200)
circle(screen, (0, 0, 0), (400, 300), 200, 2)
pygame.draw.line(screen,(0, 0, 0),(300,420),(500,420), 30)
circle(screen, (255, 3, 3), (300, 250), 40)
circle(screen, (0, 0, 0), (300, 250), 25)
circle(screen, (0, 0, 0), (300, 250), 40, 2)
circle(screen, (255, 3, 3), (500, 250), 30)
circle(screen, (0, 0, 0), (500, 250), 30, 2)
circle(screen, (0, 0, 0), (500, 250), 15)
pygame.draw.line(screen,(0, 0, 0),(200,130),(360,225), 30)
pygame.draw.line(screen,(0, 0, 0),(580,170),(440,225), 30)

pygame.display.update()
clock = pygame.time.Clock()
finished = False

while not finished:
    clock.tick(FPS)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True

pygame.quit()