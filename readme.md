20130519

A tool to test the normal layout, and some special layouts for the 9918A bitmap mode on the TI-99/4A.

Effects can be stacked, of course. Each key changes ONLY the register or mask listed below.

KEY EFFECT               Reg     Order of character sets on screen

1 - one pattern table   (4 = 00, layout 111)
2 - two pattern tables  (4 = 01, layout 121)
3 - two pattern tables  (4 = 02, layout 112)
4 - three pattern tables(4 = 03, layout 123)

5 - one color table     (mask 0, layout 111)
6 - two color tables    (mask 1, layout 121)
7 - two color tables    (mask 2, layout 112)
8 - three color tables  (mask 3, layout 123)

9 - sprites on
0 - sprites off

A - 8 characters        (mask 00)
B - 16 characters       (mask 01)
C - 32 characters       (mask 03)
D - 64 characters       (mask 07)
E - 128 characters      (mask 0F)
F - 256 characters      (mask 1F)
G - 16 chars unusual    (mask 02)
H - 16 chars unusual    (mask 04)

Character and table masks are both in register 3.
The character count is per pattern table.

Sprites lay out 6 sprites, 5-10. Sprites move vertically and horizontally so that effects can be observed. In each of the groups 5-7 (no effect from masking) and 8-10 (are affected by masking), two move horizontally (one fully within the zone and one straddling a boundary) and one moves vertically.

