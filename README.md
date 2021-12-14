# Rtree-Topdown-version
Guttman's Rtree Code with Example

test.c contains the rtree construction and building functions and a test case.

**Compilation:**
gcc test.c ../libtree.a -I/fall21/librtree/librtree-master/include -lm

When RTreeSearch function encounters a hit (overlap successful with query rectangle), then library itself will call MySearchCallback function.

struct Rect rects[] = {

        {0, 0, 0, 0}, // xmin, ymin, xmax, ymax (for 2 dimensional RTree)

        {8, 5, 8, 5},

        {7, 5, 7, 5},

        {7, 8, 7, 8},

};

Search rectangle: {6, 4, 10, 6}

Result of query:
nrects = 4

Hit data rect 1

Hit data rect 2

Search resulted in 2 hits

Note: In test.c, change #include "index.h"   to     #include "../include/index.h"
