# bouncy-squid
Building AI course project
If you need to use links, here's an example:
[Twitter API](https://developer.twitter.com/en/docs)

# bouncy-squid

Building AI course project

# Project Title

The final project for the Building AI course

## Summary
BouncySquid is an application that helps people manage domestic storage at home and exhibit their carefully selected belongings, hoping to tune their shopping habits to a level that on the one hand, of no waste and no compelled purchase; on the other hand, aligns well with our needs. 


## Background

It's quite common that endless recommendations on social media and coupons offered by e-commerce platforms seduce us to buy things that fail to align with our needs severely. And COVID-related policies have also formed our attachment to overload stockpiles which may expire. 
For those consumables, such as food, ingredients, and groceries, managing is vital.
For those collections, such as clothes, shoes, and accessories, exhibiting is important.

Fortunately, online records and offline receipts enable us to list domestic storage at home effortlessly; phone cameras also make it possible to capture our collections and recreate their brilliance.

With regular management and fancy exhibitions, Bouncy-squid is going to solve these problems:
* food wasting
* groceries expiring
* passive purchases
  

## How is it used?

There are at least 4 using scenarios.

1/ When receiving new coupons or noticing that shampoos are on a great sale, check out if you can afford a new supply based on your own pace.
Bouncy Squid will calculate your pace and give suggestions based on your purchase records.

2/ When making meal plans for the next week, take the remains in your refrigerators and stocks into consideration.
Bouncy Squid will tell their lifespans and recommend recipes accordingly for you.

3/ When fashion recommendations reach you, check if the new item is compatible with your wardrobe.
Bouncy Squid will categorize your clothes automatically and display them wisely according to categories/ colors/seasons/ weather.

4/ When you feel lacking in clothes at the beginning of a new season or have trouble deciding the garment that accommodates the temperature, check the possible collocations your old babies represent.
Bouncy Squid will suggest collocations and generate fancy photos of them in multiple actual scenes.

To make it happen, here are key using processes：

1/Make inventory lists and create display shelves
2/Check remains and restocking suggestions 
3/Review your wardrobe in different ways
4/Check possible collocations suit the weather


## Data sources and AI methods

These data are required:
* items' information, from users or e-commerce platforms
* nutrition knowledge， from https://www.webmd.com/diet/healthtool-food-calorie-counter
* food preservation knowledge, from https://nchfp.uga.edu/

| Syntax      | Description                 |
| ----------- | --------------------------- |
| Tittle      | item name                   |
| Category    | meat/vegetable/...          |
| Expiration  | 3/7/30 days, 0.5/1/6 months |
* fashion formulas, from users and bloggers they follow
* weather information, from https://www.theweathernetwork.com/ca

| Syntax      | Description          |
| ----------- | -------------------- |
| Header      | Number               |
| Paragraph1  | Winds of level 1/2/3 |
| Paragraph2  | Sunny/Rainy/Cloudy   |
* streetscape pictures, from https://unsplash.com/
* model pictures, from https://unsplash.com/
* recipes, from https://www.foodnetwork.com/recipes, https://www.bilibili.com/

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Ingridients | Text        |
| Description | Text        |

* fashion covers and pictures, from https://www.pinterest.ca/gillhams/fashion-magazine-covers/

These AI methods are required:
* convolutional neural networks, to recognize items from pictures
* the nearest neighbor classifier, to categorize items

## Challenges

Firstly, cooperation with e-commerce platforms is required to reduce user inputs when making inventory lists;
Secondly, editors both of the culinary part and the garment part are required to guarantee the quality of suggestions, and also, to avoid repeated content at first;
Thirdly, BouncySquid only helps people maintain interest in and become familiar with their wardrobes but has no plan to replace bloggers or fashion icons people are into. For example, we give collocation clues, such as color coordination, but not exactly perfect outfits; 
Moreover, it might be expensive to purchase pictures of fashion icons/shows/magazines as training data.

## What next?

Making proper suggestions, not being too pushy or too loose, and giving people a sense of achievement are the next two steps.

To make more accurate recommendations, inviting users to give personal input is necessary. Here are possible strategies:
* Keep an entry open or weekly/monthly ask users to share pictures of fashion content and self  with us as training data
* Give an initial fashion style or diet style diagnosis to each user and then change the diagnosis as they keep sharing.

To form a sense of achievement for users, informing and identifying changes are necessary. Here are possible strategies:
* Weekly generate movies using resources each user provides, i.e., their #ootd photos or pictures of fashion content.
* Identify and trace nutrition distributions of their meals, and then visualize changes. 


## Acknowledgments

* list here the sources of inspiration 
* do not use code, images, data etc. from others without permission
* when you have permission to use other people's materials, always mention the original creator and the open source / Creative Commons licence they've used
  <br>For example: [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org/wiki/File:Sleeping_cat_on_her_back.jpg#filelinks) / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
* etc
