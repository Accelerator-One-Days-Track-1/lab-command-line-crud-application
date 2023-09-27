# Command Line CRUD Application

You will build an application that lets users round up the change for each purchase and set it as a donation.

## Getting Started

1. Fork and clone this repository
1. Open up the repository in your code editor.
1. Start a new node project
1. Set up a .gitignore file
1. Install nanoid version 3
1. Install chalk version 4

## Instructions

Build out the following functionality. Be sure to organize your code so that the functions stay small and have one job, and also, manage your files so that it is clear what kind of functions are within each file.

- A user can `create` a purchase. The purchased object will have the following:
  - `id` - generated by nanoid
  - `name` - the name of the purchase
  - `amount` - the purchase amount
  - `donation` - the donation amount, rounded to two decimal places
- A user can see an `index` of all their purchases, showing the `id` and the `name`.
- A user can see a `show` view with all the purchase details using the `purchase id`. This view should have additional styling (see below).
- A user can `update` the amount of a purchase using the `purchase id`.
- A user can `delete` a purchase using the `purchase id`.
- A user can see the total amount of donations from the `sum` of all purchases.

Here is an example of additional styling for the show view

![Additional styling for the show view](./assets/show-view.png)

Include Jest, and write a minimum of two tests. You could:

- Confirm all the correct fields exist when creating a new item.
- Make sure the correct datatype is being inserted into each field.

With the following functionality, you would likely want to make a sample data set that is always the same (you can create a small array of objects (~2-3 items) that is hard-coded in your test file, or you can create a separate file and import it). You would not use the `fs` module to update any changes permanently. You can look for examples of using sample data with a previous lab you have completed.

- Confirm that the function to create one item creates only one item and appends it to the test array.
- Confirm that the delete function deletes the correct object in the test array.
- Confirm that the edit function edits the correct object in the test array.
- Confirm that the output for the show view matches your expected output.
- Confirm that the output for the index view matches your expected output.

## Bonus

Instead of your user remembering the order to enter data. Upgrade your functionality so your user can create key-value pairs and then the user can input them in any order:

```
npm run update amount="4.44" name="Mechanical Pencil" id=rSl_
```
