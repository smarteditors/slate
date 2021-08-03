# Items

Items are phycical assets, for example chairs in an office or store. Items belong to Catalogue Items (see Catalogue Items end points), which are analagous to models.

The Item class stores granular information on an item, such as colour, sale and purchase information, and warranty information. 

In addition to data stored directly on the Item class, Items also store data on Item Attribute associations.  

 Items belonging to Catalogue Items often share similar attributes, for example they may all be made from the same material. Where there is no variation of an attribute between Items that belong to a Catalogue Item, the attribute data is stored as an association on the Catalogue Item, rather than on each of the Items. For example, Items belonging to a Catalogue Item named 'Office chair' could all be of the same size, in which case the size would be stored as an Attribute associated to the Catalogue Item. however some could be black and some could be blue, in which case a colour Attribute would be stored as an association on each of the Items.
