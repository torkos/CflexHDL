#Led glow<br>
cd led_glow && make<br>
SIMULATION RESULTS: Average duty cycle: 49%, clock frequency 437 MHz<br>

#Graphics demos<br>
cd demos/vga<br>

**Pergola's ROTOZOOM:**<br>
![image](https://user-images.githubusercontent.com/8551129/196615024-e890c3fa-6fb1-49be-b37e-ab7f29763734.png)<br>

make VGA_SRC=build/migen_vga.cc clean all<br>
FPS 503.3, pixel clock 154.6 MHz (simulation)<br>
FPS 181.5, pixel clock 55.7 MHz (verilator)<br>

**Silice's FLYOVER 3D:**<br>
![image](https://user-images.githubusercontent.com/8551129/196614548-fd2ee539-0427-47b6-b9b3-d4dd9885be80.png)<br>

make clean all<br>
FPS 642.3, pixel clock 197.3 MHz (simulation)<br>
FPS 132.4, pixel clock 40.7 MHz (verilator)<br>

**LiteX's COLORBARS:**<br>
![image](https://user-images.githubusercontent.com/8551129/196614509-781472c2-bea5-4dcf-8512-76ab8a9d444d.png)<br>

make VGA_SRC=build/migen_vga.cc MIGEN_VGA=litex_vga.py clean all<br>
FPS 713.5, pixel clock 219.2 MHz (simulation)<br>
FPS 139.5, pixel clock 42.9 MHz (verilator, needs manual patch)<br>