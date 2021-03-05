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

# Day 7 Functions and data cleaning

Everything in Dot's new house is finally coming together now! The repairs are finished, and the cleaning's done. But the house won’t feel like a home until Dot finishes unpacking all their belongings. The problem is, the way things are organized is so chaotic that every time Dot approaches the pile of their boxes, they get overwhelmed and run away to continue procrastinating.

Help Dot stop procrastinating on unpacking their things by cleaning up the dataset of their belongings.

Dot has a lot of different boxes laying around. They need a system for how to unpack them, or they'll just continue procrastinating. Help Dot sort the boxes by their weight.

           Box:	Weight (kg)
           Box 1	4
           Box 2	2
           Box 3	18
           Box 4	21
           Box 5	14
           Box 6	13

Create a function that will open the boxes according to their weight, from lightest to heaviest.

# Day 8 Data Frames

Dot had a tiring set of days last week, getting their new off-the-grid home repaired and tidied up. Last night they sure slept like a log, if logs could sleep. Waking up well-rested to a sparkling-clean home, they feel completely rejuvenated and happy. 

When pouring some milk into their morning coffee, an idea starts whirring in Dot's head. They live in a rural place now, why would they continue buying milk at the grocery store like a city-dweller? Why not get it directly from a cow? 

Dot knows that there's a big cow farm just down the road where you can rent out a spotted friend for a few months. The thing is, they're not sure if this is the best time to do that. Do cows produce more milk during certain months, and less during others? 

By analyzing the dataset with pandas, answer the following questions for Dot:

At what year and month did company x produce the most milk?
At what year and month did company x produce the least milk?
           
           import pandas as pd

           #To Read a Dataset
           #Milk.csv is stored into a Pandas DataFrame variable called df.
           df = pd.read_csv('milk.csv')

# Day 9: pandas data cleaning & filling NaNs

Dot understands how cows work a bit more now. They got themselves really hyped up to rent a cow, and traversed down the road to the cow farm. Dot spent some time negotiating with the cow farmer how much it would be to rent a cow, then went over to take a look at the beasts and pick a favourite.

Examining the moo-ing creatures, a realization slowly sinks in. If Dot did rent out a cow, they would definitely get attached to it over the month. Having to give it back to the farmer would be heartbreaking! They think back to their youth, when they briefly took care of a friend's plankton. Giving the plankton back was one of the saddest moments of their life.

Maybe Dot isn't thinking big enough. What if they took a leap and bought an entire cow - would it be worth it? How much milk would they get out of it?

Fill out the missing values in the monthly milk production column with the median, and fill out the number of cows column using the ffill method.

After filling in the missing values with our new data, answer these questions for Dot, so they can figure out the value of having a cow year-round:

What is the average for monthly milk production?
What is the standard deviation for monthly milk production?
What is the average number of cows used?
           
           import pandas as pd
           df = pd.read_csv('milk_2.csv')

# Day 10: pandas data modification

Dot shakes hands with the farmer after finalizing the purchase of the most beautiful cow on the farm, who's name is Bessie. They bring Bessie over to their cabin and set her up on the front lawn. Dot stares into the eyes of their new four-legged friend, envisioning all the good times they might have. Eating grass. Standing. Sleeping. Staring blankly into the distance. What a life they could have together!

But, another thought is starting to bother Dot...they're just one person, and they're not sure how much milk they'd be able to drink. They like putting dairy in their coffee and cereal just as much as anyone else, but drinking a tall glass of milk on its own kinda grosses them out.

What are they gonna do with all this milk? Ah-ha - maybe they can sell it! But how profitable will that be?

Help Dot figure out how profitable selling fresh milk can be, by looking at the dataset for the cow farm. Fill in the values for the following columns based on the available data:

Total Milk Production
Total Revenue

           import pandas as pd

           df = pd.read_csv('milk_32.csv')
           df = df.drop(columns = ['Unnamed: 0'])
