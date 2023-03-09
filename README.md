# Seven-Nation-Army

use_bpm 120
use_synth :fm
use_synth_defaults sustain: 0.25
beats = [:e3,:e3,:g3,:e3,:r,:d3,:c3,:b2]
sleep = [1.5,0.5,0.75,0.25,0.5,0.5,2,2]
x=0
y=0
live_loop :white_stripes do
  8.times do
    play (beats [x])
    sleep (sleep[y])
    x= x+1
    y= y+1
  end
  x=0
  y=0
end
