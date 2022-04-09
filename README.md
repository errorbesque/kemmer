kemmer 5

exploring possibilities and limitations of projection mapping with mapper.js
old project: https://glitch.com/dashboard?group=owned&sortColumn=boost&sortDirection=DESC&page=1&showAll=false&filterDomain=


to try in quads:
video  
shader
hydra

to implement:
multiple of those ^ with fft responsivity

backup plan... just projection i guess? like it'd be cool if hydra could automatically cycle through some things. 

lagginess happens and chrome often crashes. checking if running this locally will help... 

hm nm should i try to learn touchdesigner instead?
hm apparently the noncommercial version is free so i guess i'll at least try it

KantanMapper
For this tutorial we’ll be focusing on KantanMapper, which is the most straightforward of the tools and often has enough functionality to solve most situations. If you’re interested in mapping to more complex geometry for which you have a digital model, check out camSchnapper.

look for mirabelle's demo lol.

done with establishing kantan (thanks wolves)

TouchDesigner

visualizations to switch between

_ make another viz (particle tutorial)
-- stuck on opencl thing, try restarting
X increase framerate of blended images
_ get more images to blend
_ change filenaming (to %02d) in the new folder

_ observe playback on very slow speed
-- currently with settings (60fps, speed = .022) we do about 1 image a minute
to fill an hour you'd need 60 images (easy i guess?)


input01="img0 - %01d.jpeg"

ffmpeg -y -fflags +genpts -r 120 -i $input01 -vf "setpts=100*PTS,minterpolate=fps=120:scd=none" -pix_fmt yuv420p "test02.mp4"


