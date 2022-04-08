# Lab 6

I started with the getting started tutorial to learn a bit about the libraries we are using.

The first part of this lab was working properly for me.
![part-1.png](part-1.png)

## Word ladder

### Bullet point 1

Lines 80 to 82 I changed to the following:

```python
for (source, target) in [('chaos', 'order'),
                             ('plots', 'graph'),
                             ('moron', 'smart'),
                             ('flies', 'swims'),
                             ('mango', 'peach'),
                             ('pound', 'marks')]:
        print("Shortest path between %s and %s is" % (source, target))
```

The full version is stored in word-ladder.py.

My output was:

```
Loaded words_dat.txt containing 5757 five-letter English words.
Two words are connected if they differ in one letter.
Graph has 5757 nodes with 14135 edges
853 connected components
Shortest path between chaos and order is
chaos
choos
shoos
shoes
shoed
shred
sired
sided
aided
added
adder
odder
order
Shortest path between plots and graph is
plots
plats
plate
prate
grate
grape
graph
Shortest path between moron and smart is
moron
boron
baron
caron
capon
capos
capes
canes
banes
bands
bends
beads
bears
sears
stars
start
smart
Shortest path between flies and swims is
flies
flips
slips
slims
swims
Shortest path between mango and peach is
mango
mange
marge
merge
merse
terse
tease
pease
peace
peach
Shortest path between pound and marks is
None
```

### Bullet point 2

For the next part, I changed line 61 from `fh = gzip.open('words_dat.txt.gz', 'r')` to `fh = gzip.open('words4_dat.txt.gz', 'r')`, line 67 from `w = str(line[0:5])` to `w = str(line[0:4])`, and then changed lines 80 through 85 again to:

```python
for (source, target) in [('cold', 'warm'),
                             ('love', 'hate'),
                             ('good', 'evil'),
                             ('pear', 'beef'),
                             ('make', 'take')]:
        print("Shortest path between %s and %s is" % (source, target))
```

The full version is stored in word-ladder-4.py.

My output was:

```
Loaded words_dat.txt containing 5757 five-letter English words.
Two words are connected if they differ in one letter.
Graph has 2174 nodes with 8040 edges
129 connected components
Shortest path between cold and warm is
cold
wold
word
ward
warm
Shortest path between love and hate is
love
hove
have
hate
Shortest path between good and evil is
None
Shortest path between pear and beef is
pear
bear
beer
beef
Shortest path between make and take is
make
take
```

### Bullet point 3

In `edit_distance_one`, I added this at the beginning:

```python
for tmp in it.permutations(word, 5):
            newWord = ''.join(tmp)
```

and then based all of the calculations within that function off of the `newWord`, instead of `word`.

The full version is stored in word-ladder-permutation.py.

My output was:

```
Loaded words_dat.txt containing 5757 five-letter English words.
Two words are connected if they differ in one letter.
Graph has 5757 nodes with 112278 edges
16 connected components
Shortest path between chaos and order is
chaos
chose
chore
coder
order
Shortest path between plots and graph is
plots
opals
plash
sharp
graph
Shortest path between moron and smart is
moron
manor
roams
smart
Shortest path between flies and swims is
flies
isles
semis
swims
Shortest path between mango and peach is
mango
conga
nacho
poach
peach
Shortest path between pound and marks is
pound
mound
monad
moans
roams
marks
```