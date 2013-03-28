# Crossing The Refactoring Swamp

## by Ken Mayer

### Abstract

Refactoring can be hard to balance against the urge to dive right back into delivering features. The good news, though, is that refactoring can take place anywhere. It can be done solo. It can be done in pieces. Recently, when I needed to refactor an annoying patch of code, I worked on it during my daily commute to and from the office. It didn’t interfere with client work or family time, and I accomplished a significant amount of work with near-zero opportunity cost.

### Additional Notes

#### Red-Green-Refactor Without Refactor Is About As Useful As a Two-Legged Stool

The test-driven development “mantra” is red ➔ green ➔ refactor ⟲. It is an essential step in the development process. Without it, over time, your code will accumulate unnecessary dependencies, have poor separation of responsibilities, and present confusing interfaces; all the opposite of SOLID design.

#### Technical Debt Is Like a Payday Loan

It is quite easy to be seduced to the dark side where you get to “green” and then decide to refactor “later,” where later often never comes. This decision is like a payday loan. You are incurring technical debt every time you deliver a new feature. And as is true for payday loans, your velocity will appear to be faster, but just a few iterations down the road, the debt must be paid. Eventually, your velocity will start to bog down, developers will cringe when they have to edit the code, tests will become brittle, and finally, refactoring will no longer be an option. The only choice will be to declare “bankruptcy”; that is, rewrite the code from scratch. That is why it is so important to complete the refactor within the context of a feature.

#### About The Author

Ken is a serial technologist and open source advocate. He discovered Ruby on Rails *almost* by accident in 2007 and knew instantly that this was a technology and philosophy worth pursuing. He is a sporadic blogger; an unpredictable tweeter; a recovering SCUBA instructor and an erstwhile master of vessels steam and sail; most of all, he's a devoted husband and father. His sons thinks he's cooler than anything.

## Social

* [http://pivotallabs.com/author/ken](http://pivotallabs.com/author/ken)
* [@kennethmayer](http://twitter.com/kennethmayer)
* [https://github.com/kmayer](https://github.com/kmayer)
