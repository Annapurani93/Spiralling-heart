library(jasmines)
library(magrittr)
library(dplyr)
library(ambient)
library(ggplot2)
library(gganimate)
library(magick)

entity_heart(seed = use_seed(300), 
             grain = 300, 
             shape=heart,
             start=0,
             end=300)%>% 
  unfold_breeze(iterations=3,
                scale=0.01,
                drift = 0.01)%>%
  style_walk(palette = palette_manual("blue"), 
            colour = "blue", 
            background = "black")->h1

h1

anim_save("C:/Users/Annapurani/Desktop/h2.gif", h1)
image_read('C:/Users/Annapurani/Desktop/h1.gif')->hb
hb%>% image_annotate("@annapurani93", size = 8, color = "white", location = "+400+460")->new
image_write(new, "heart.gif")
