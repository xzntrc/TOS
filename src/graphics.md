# Graphics in TempleOS
King Terry in his divine widom not only programmed the entire operating system singlehandedly, but also programmed in libraries for 2D and 3D graphics.

There are a couple of essential things to know about when programming graphics in TempleOS:

- DeviceContext (mostly seen as dc in code)
- Gr- functions
- Fs properties

In TempleOS, you have full control over all graphics operations. However, there are some niceties that Terry graciously provided to make writing games and graphical applications easier.

## Fs->draw_it
If you look at the example games Terry made, you will find that many of them have a line like this:
`Fs->draw_it=&DrawIt;`

> Fs is a pointer to the current task. The class representing the task is called a CTask. Type CTask into the terminal and hit `CTRL+SHFT+F1` to inspect the code.

The draw_it member variable is a function pointer that makes our lives easier. It calls whatever function it points to every frame and clears the screen of graphics before drawing again.

In most of Terry's programs, he makes a function called DrawIt that manages all graphics. In order to use the Fs->draw_it function pointer, your DrawIt function must have two parameters: a CTask and a CDC. Your function declaration should look something like this:

```U0 DrawIt(CTask *task, CDC *dc) {```

The dc variable is extremely useful for graphics. 

Just before we get to some common drawing functions, let's see what a Main() function would look like.

```
U0 Main()
{
    SettingsPush;
    DocClear;
    Fs->draw_it=&DrawIt;
    while(!GetChar) Yield;
    SettigsPop;
}
Main;
```

Let's take a look at some graphics functions.

# Graphics Functions
Most graphics functions can be found in this file:
`C:/Adam/Gr/GrBitMap.HC.Z`

Useful functions:
- Sprite() 
- GrPrint(CDC *dc, I64 x, I64 y, U8 *fmt, ...)
> x and y correspond to the (x,y) position for the text to appear on screen.
> This function works as a way to print a formatted string to the screen. Type something like "%s" into the fmt argument, and place strings or variables after that.
- GrRect(CDC *dc, I64 x, I64 y, I64 w, I64 h)
- GrCircle(CDC *dc, I64 centerX, I64 centerY, I64 radius)
- GrEllipse(CDC *dc, I64 centerX, I64 centerY, I64 x_radius, I64 y_radius, F64 rot_angle=0)
- GrLine(CDC *dc, I64 x1, I64 y1, I64 x2, I64 y2) {
> GrLine and GrEllipse have more parameters you can go check out.

