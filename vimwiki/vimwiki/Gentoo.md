
# Captura vídeo y audio
ffmpeg -video_size 1366x768 -framerate 25 -f x11grab -i :0.0+,30 -f pulse -i default -ac 2 screencast.mp4

## Captura simple
ffmpeg -f x11grab -i :0.0 out.mkv

## Captura pantalla y audio mic 
ffmpeg -f x11grab -framerate 60 -i :0.0 -f alsa -i default out.mkv

# Formatear Fat32
sudo mkfs.vfat -F 32 -n Mi_Memoria /dev/sdc1

# Seleccionar Captura 
maim -s -u screen.png



