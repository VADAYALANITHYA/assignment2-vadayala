#assignment2-vadayala
# nithya vadayala
###### COPENHAGEN
Copenhagen is the capital and largest city of denmark, on the east coast of the country. According to several specailised sources, the city has a population of approximately of **1.3 million  inhabitants** 
copenhagen is the administrative ,cultural and commercial center of denmark. The city is one of the important tourist attraction all over the world,particulary in europe. Tivoli gardens was opened back in 1843, and since then it has entertained national and forigen visitors alike.

---

# Directions from Maryville to Copenhagen
1. It covers a distance of 10,000 miles from Maryville to Copenhagen through airport
2. Catch a cab and go from Maryville to kansas city airport.
    1. first flight from kansas to Newyork
    2. After reaching to Newyork, change your flight to london heatthrow
3. We have a layover for 12 hours
    1. Next flight from london to Denmark
    2. After reaching Denmark take a train to Copenhagen
4. Finally we reach our destination

* I would like to carry:
    * Accessories:
        * Camera
        * HandBag
        * Earphones
    * Drinks:
        * Fanta
        * MinuteMaid
    * Snacks:
        * Biscuits

**[AboutMe.md](AboutMe.md)**

---

# My favourite food that I will suggest for others to try
 I am going to create a table with atleast 4 food items. My favourite food items are chicken shawarma, vegetable biryani,Butter naan,ice kheer and Gulab jamun.

 |food item|location|cost|
 |---|---|---|
 |chicken shawarma|Paradise|10$|
 |vegetable biryani|bawarchi|5$|
 |butter naan|srikanya|2$|
 |rice kheer|ratna|5$|
 |gulab jamun|hyvee|6$|

---

# Pithy Quotes

>"life is journey not a destination."-*Radalph*<Br>
> "Not all who wander are lost."-*JRR*

---

# SQRT decomposition

>A SQRT decomposition is a data structure that allows answering range queries over an array effectively, while still being flexible enough to allow modifying the array. This includes finding the sum of consecutive array elements  or finding the minimum element in a such a range in time. Between answering such queries the Segment.

[Click here to know more](https://en.wikipedia.org/wiki/SQRT_meldabe_decomposition)

```
// input data
int n;
vector<int> a (n);

// preprocessing
int len = (int) sqrt (n + .0) + 1; // size of the block and the number of blocks
vector<int> b (len);
for (int i=0; i<n; ++i)
    b[i / len] += a[i];

// answering the queries
for (;;) {
    int l, r;
  // read input data for the next query
    int sum = 0;
    for (int i=l; i<=r; )
        if (i % len == 0 && i + len - 1 <= r) {
            // if the whole block starting at i belongs to [l, r]
            sum += b[i / len];
            i += len;
        }
        else {
            sum += a[i];
            ++i;
        }
}
```

[Code Source](https://cp-algorithms.com/data_structures/segment_tree.html)
