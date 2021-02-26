# 21daychallenge2021
21-Day Python Data Science Challenge with Lighthouse Labs starting February 17th: https://data-challenge.lighthouselabs.ca/

## Day 1 Sign the lease using string formatting

Challenge: Modify the lease agreement with your signature without changing the original lease variable.

           lease = '''Dear Dot, 
                      This document validates that you are beholden to a monthly payment of rent for this house.
                      Rent is to be paid by the first of every month.
                      Fill in your signature to agree to these terms.  
                       -------------
                       Please Sign Here: 
           '''

## Day 2 Grocery Price Percentage Difference

Dot has a few lists you can use as reference: their grocery list, the prices they used to pay in the city, and the prices for the rural grocer. What is the price difference between groceries in the city vs. groceries in the country, as a percentage of country prices?

## Day 3 lists, dictionaries and indexing

Dot has some specific rules for what they want to change in the shopping list:

They hate oak wood, and prefer maple.
They want to paint all the rooms blue except the kitchen, which they want to paint white.

           old_blueprint = {
               "Kitchen": ['Dirty', 'Oak', "Damaged", "Green"],
               "Dining Room": ['Dirty', 'Pine', 'Good Condition', 'Grey'],
               "Living Room": ['Dirty', 'Oak', 'Damaged', 'Red'],
               "Bedroom" : ["Clean", 'Mahogany', 'Good Condition', 'Green'],
               "Bathroom": ["Dirty", 'White Tile', 'Good Condition','White'],
               "Shed"    : ['Dirty', "Cherry", "Damaged", "Un-painted"]
           }

           shopping_list = ['20 x Oak Plank', '20 x Oak Plank', '20 x Cherry Plank', 'White Paint', 'White Paint', 'White Paint']
Note: The blueprint above is in a dictionary format and we won't be needing to work with dictionaries in the challenge, use the blueprint as reference only.

Use python's pop(), insert(), and append() list functions to change the shopping_list above so that it reflects the right materials needed.

The list should be ordered by wood types first, then paint types.

           example_shopping_list = ['wood type in room A', 'wood type in room b','paint type in room a','paint type in room b']
Create a paint_list list from the new_shopping_list list using the built in python list indexing ability.

## Day 4 Wholesale vs Retail Price comparison using for-loops

Dot needs to purchase:

600 planks of Oak Wood
150 liters of Blue Paint
15 liters of White Paint
165 liters of Paint Finish


Item	Needed Amount to Buy	Wholesale Price	Retail Price
Plank of Oak Wood	600	$ 7000	$ 12.99
1 Liter of Blue Paint	150	$ 1000	$ 8.99
1 Liter of White Paint	15	$ 1000	$ 9.99
1 Liter of Paint Finish	165	$ 800	$ 3.99


Use a loop to determine the price Dot would pay for purchasing supplies at the retail price. Based on that calculation, which itmes should Dot buy at retail vs. wholesale?

Note: Assume the wholesale price covers all the supply Dot needs for each item, whereas the retail price is per single unit.

           item_list = ['Oak Wood', 'Blue Paint', 'White Paint', 'Paint Finish']

           amount_list = [600,150,15,165]

           wholesale_price_list = [7000, 1000, 1000, 800]

           retail_price = [12.99, 8.99, 9.99, 3.99]

## Day 5 Conditional Logic and Control Flow

Dot's okay with paying a bit of a surplus for convenience, but they don't want to go broke buying dustpans and glass cleaner. Help them figure out which items cost over 10% more at the nearby store, so they can avoid buying these items.

Using Python, develop a list of items that are too expensive for Dot to purchase at the nearby store.

           # Cleaning Supplies List (19 items)
           cleaningsupplies_list = ['Broom', 'Mop', 'Dustpan', 'Garbage Bags', 'Glass Cleaner', 'Vinegar',
                                   'Soap', 'Bleach', 'Duster', 'Floor Cleaner', 'Sponges', 'Dish Soap',
                                   'Drain Cleaner', 'Paper Towels', 'Cleaning Rags', 'Toilet Cleaner', 
                                   'Rubber Gloves', 'Alcohol Wipes', 'Squeegee']

           # City Price
           city_price = [6.49, 4.99, 3.39, 4.29, 3.99, 1.99, 
                         1.50, 3.99, 4.99, 5.99, 2.99, 2.99, 
                         5.99, 2.99, 3.49, 6.99, 2.99, 1.98, 11.99]

           # Country Price
           country_price = [5.49, 4.69, 4.42, 5.99, 5.99, 2.50,
                           1.25, 2.49, 4.50, 6.75, 2.49, 1.99, 
                           6.25, 3.99, 3.59, 4.99, 1.69, 1.87, 10.99]

## Day 6 Descriptive Statistics with Pandas Library

Challenge:
There are many holes in the living room's ceiling that desperately need to be fixed. Dot's measured them, and in total there are about 100. They need to figure out how much does it cost to fix all of the holes. Differently sized holes will require differently sized patches to fix them.

           Size of Hole	                                 Cost to Fix
           Small (less than 20 mm)	                              $1.30
           Medium (above or equal to 20 mm AND less than 70mm)    $1.60
           Large (above or equal to 70 mm)	                      $2.10
Dot needs you to look at the measurements and figure out the answers to the following questions:

Using pandas, determine:
What is the average sized hole?
What is the average cost to fix a hole?
What is the total cost of fixing all of the holes?
