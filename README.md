# 🧑‍💻 Planity test

Rendering appointments on a timeline with 2 constraints.
This algorithm find the proper width for every appointment
and then packs them in the timeline.
The algorithm is O(n²×log(n)) where n is the number of appointments.

## 🧠 Algorithm overview

The algorithm will find clusters of overlapping appointments
and check for every time slot the number of overlapping appointments
for this cluster. The maximum will be the width fraction
of each appointment of the cluster.
Then, for each appointment, the algorithm will find the first free place
among the overlapping appointments already placed.

## ❔ Why vanilla JS?

To be honest I felt like the main focus was on the algorithm
(which took me some time to figure out) so I didn't wanted to add libraries
or frameworks to the mix. Just the algorithm and the rendering.
Also I wanted to share it easily so one just need a browser and then can run it.

## 🧱 Structure

It is only an index.html file.

The HTML has a script tag with the algorithm and the rendering function.
The rendering function creates the appointments in the div#appointments.

## 🚀 How to run

Just open the index.html file in a browser.
