# trigger tidbits
Intersting stuff that trigger my imagination


## TB of the day

10 Nov 2021: Performance in a ditributed service world

I recomend reading this article around throttling realtime events in the browesr to improve performace and not overload either the or backend service
https://css-tricks.com/debouncing-throttling-explained-examples/

Although this article refers to performance considerations in browser embedded JavaScript, the principles are particularlary relevent in building any realtime or event based system. 

The topics covered in this article are are very relavent when you have a hybrid setup where some part of your application stack `is batch driven` and another connected part is `realtime`.

Here are some examples:
1.  Creating a UI with a typeahead input which makes an call to a backend api that populates the dropdown on each keystroke.
2.  Introducing a websocket stream that pushes price updates to a browser and triggers a grid to make a backend api call to refresh.
3.  Integrating a datastream e.g. Kafka that triggers processing in your service application, then on each update your application makes a further call to another (micro)service on every Kafka message.

You can immagine a host of further examples where either the rate of event triggers in the environment that generates events and downstream services which are impacted on can not keep up.

#### Interesting, does this trigger your thoughts

