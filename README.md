# Product-Pricing-System
The program calculates selling prices for a company handling elementary and composed products.Elementary products have purchase prices, while composed products incur fabrication costs. Prices for composed products are computed by considering both constituent prices and fabrication costs.

# More details:
We aim to develop a Python program to determine selling prices for a company that purchases elementary products for use in the production of other composed products. In this information system, a product can be either elementary or composed. For each composed product, its composition (or constitution) needs to be known, i.e., the elementary products involved in its production along with their quantities.

# Classes to Define:

_Composition Class:

Two private attributes __produit and __quantité.
A constructor with two parameters.
Getters and setters for the attributes using the @property decorator.

_Produit Class:

Two private attributes __nom and __code.
A constructor with two parameters.
Getters for the attributes using the @property decorator.
An abstract method getPrixHT.

_ProduitElementaire Class:

A private attribute __prixAchat.
A constructor.
A __str__ method returning information about an elementary product.
A getPrixHT method returning the prixAchat of an elementary product.

_ProduitCompose Class:

A private attribute __fraisFabrication, representing the cost incurred in the production of a product from its constituents (the value of constituents is not considered).
An attribute tauxTVA with a fixed value of 18% for all composed products.
A private attribute `__listeContituants
__listeContituants representing an array of compositions.

A constructor.
Getters for the attributes using the @property decorator.
A __str__ method returning information about a composed product.
A getPrixHT method calculating and returning the price excluding tax, which is the sum of the prices excluding tax of all constituents plus the fabrication costs of the product.
# Testing:
In a file named main.py, test all the implemented classes and methods to ensure the proper functionality of the product pricing system.
