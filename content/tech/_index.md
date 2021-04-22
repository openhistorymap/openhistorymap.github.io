---
title: "Tech"
featured_image: "marvin-meyer-SYTO3xs06fU-unsplash.jpg"
---

# The Open History Map Stack

From a technical point of view we need to address the problem of history visualizaition from several points of view: 
* **the ontology of the past**: Representation of the past is not inherently easy and as such it is quite complex to map a past world into a modern day infrastructure.
* **the visualization of data considering time as a linear dimension**: This creates enormous problems when you consider a database that has typically x and y as keys for the tiles with data to be visualized. Once you add a third dimension, you have to choose between splitting time across those single tiles or splitting the tiles over time. Both ways are complicated, considering that data has to be stored in efficient ways adds issues to the structure and, finally, the data to be sent to the users is one further step of complexity to consider. For this reason we have developed our own full stack of APIs and servers for all the parts to work in harmony. All of these parts are already or will be soon open sourced in our repo (https://github.com/openhistorymap ).
* **the comparison of different moments in time and the navigation between two moments**: This is an issue we have not yet addressed, but we already have ideas about it in order to visualize how the world between arbitrary dates changed.
* **Integration of broader source data**: Photos have been invented at the end of 18th century, but mankind has painted views of the world since the beginning of time. For this reason we would like to be able to show the users the located pictures of the past, located both in space (which is quite common) and in time (more complicated).
